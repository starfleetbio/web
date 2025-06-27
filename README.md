# web

A static Jekyll-based web site served on S3 through CloudFront deployed by github actions.

``` bash
bundle exec jekyll serve -l -o
```

[ci/cd setup](https://pagertree.com/blog/jekyll-site-to-aws-s3-using-github-actions)

added ACL privs to bucket