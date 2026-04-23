---
title: "About DNAVault"
layout: single
permalink: /dnavault/about/
dnavault_site: true
show_date: false
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/header.jpg
  overlay_filter: 0.4
  overlay_color: "#0D1117"
---

## What is DNAVault?

DNAVault is a privacy-first genomics app for iPhone. It lets you explore your own genetic data — kinship, ancestry, health, and more — entirely on your device. Your genome never leaves your phone.

## Privacy by Design

Every feature in DNAVault runs locally:

- **Kinship analysis** — IBD segment comparison runs on-device. Proximity sharing is end-to-end encrypted and nothing is retained after analysis.
- **Haplogroup classification** — Y-DNA and mtDNA classification using Yleaf and mitoLEAF algorithms, on-device.
- **Health screening** — ClinVar variant lookup runs against a local database you download once.
- **Ask** — Queries are sent to Claude AI via an anonymizing proxy. Your genome data itself is not transmitted; only the text of your question and relevant extracted variants are included.

## Supported Formats

| Format | Coverage |
|---|---|
| Whole Genome Sequencing (WGS) | Full variant coverage |
| AncestryDNA raw data | ~700K SNPs |
| 23andMe raw data (v3, v4, v5) | ~600K–1M SNPs |

## The Science

DNAVault implements peer-reviewed algorithms for every analysis. See the full [Scientific References](/dnavault/references/) for citations covering kinship, haplogroup classification, health variant interpretation, and ancestry.

## Who Built This?

DNAVault is developed by [StarfleetBio](https://starfleetbio.com) — a company focused on computer-aided science for modern research and development.

Questions or feedback: [dnavault@starfleetbio.com](mailto:dnavault@starfleetbio.com)
