# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static Jekyll-based website for StarfleetBio (https://starfleetbio.com) using the Minimal Mistakes theme. The site is deployed to AWS (S3 + CloudFront + Route 53) via GitHub Actions CI/CD.

## Development Commands

### Local Development
```bash
bundle exec jekyll serve -l -o
```
This starts the local development server with live reload (`-l`) and automatically opens the site in a browser (`-o`).

### Build
```bash
bundle exec jekyll build
```
or with production environment:
```bash
JEKYLL_ENV=production bundle exec jekyll build
```

## Architecture & Structure

### Jekyll Configuration
- Theme: Minimal Mistakes Jekyll with "dirt" skin
- Config: `_config.yml` contains site-wide settings including URL, analytics, default YAML front matter
- Ruby version: Specified in `.ruby-version` file
- Dependencies: Managed via Gemfile/Gemfile.lock

### Content Organization
- **`_posts/`**: Blog posts with date-based filenames (`YYYY-MM-DD-title.md`)
- **`_pages/`**: Static pages (about, mission, work, posts, contact)
- **`_data/`**: Site data files:
  - `authors.yml`: Author profiles (vanetten, cleveland)
  - `navigation.yml`: Main navigation menu structure
- **`_includes/`**: Reusable template partials (currently empty)
- **`assets/`**: Images and other static assets
- **`index.md`**: Homepage content

### Post Front Matter
Posts require YAML front matter with:
```yaml
---
title: "Post Title"
excerpt: "Brief description"
date: YYYY-MM-DD HH:MM:SS -0400
author: vanetten  # or cleveland (defined in _data/authors.yml)
---
```

### CI/CD Pipeline
The `.github/workflows/build_and_deploy.yml` workflow:
1. Triggers on push to `main` branch
2. Sets up Ruby environment
3. Builds Jekyll site with production environment
4. Syncs `_site/` to S3 bucket
5. Invalidates CloudFront cache
6. Notifies Google of sitemap update

Required GitHub secrets:
- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_S3_BUCKET_NAME`
- `AWS_CLOUDFRONT_DISTRIBUTION_ID`

### Theme Customization
This site uses the Minimal Mistakes theme. Default layouts and configuration options are documented in the [Minimal Mistakes default config.yaml](https://github.com/mmistakes/minimal-mistakes/blob/master/_config.yml).

Site-wide defaults in `_config.yml` set:
- Layout: `single`
- Author profile: enabled
- Date display: enabled
- Width: `wide`
- Header image: `/assets/images/header.jpg`

## Workflow Notes

- The site automatically deploys to production when changes are pushed to `main`
- The build process excludes `TODO.md` and `README.md` from the final site
- CloudFront caching is set to 7 days (604800 seconds) with invalidation on each deploy
