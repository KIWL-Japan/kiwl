# KIWL Jekyll Site

This repository contains a Jekyll site for KIWL, a charity group raising funds for Mirai no Mori.

## Local Development

Install dependencies:

```sh
bundle install
```

Run the site locally:

```sh
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`.

## GitHub Pages Deployment

The workflow at `.github/workflows/deploy.yml` builds the Jekyll site and deploys it to GitHub Pages when changes are pushed to the `main` branch.

In the repository settings, set GitHub Pages to use **GitHub Actions** as the source.
