# KIWL Jekyll Site

This repository contains a Jekyll site for KIWL, a charity group raising funds for Mirai no Mori.

## Local Development

Use the Ruby version in `.ruby-version` (currently 3.4.13). The deployment workflow reads this file too, so Ruby updates only need to be made in one place.

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

Pull requests to `main` run the production Jekyll build through `.github/workflows/check.yml`. This check uses the site's `/kiwl` base path and does not deploy. Both workflows use the Ruby version in `.ruby-version`.

In the repository settings, set GitHub Pages to use **GitHub Actions** as the source.

The published site is at https://kiwl-japan.github.io/kiwl/.
