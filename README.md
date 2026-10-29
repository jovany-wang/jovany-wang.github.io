# jovany.wang

Personal site of Qing Wang (Jovany), built with [al-folio](https://github.com/alshedivat/al-folio) v1.2 and published to GitHub Pages at [jovany.wang](https://jovany.wang).

Posts live in `_posts`. Unpublished drafts live in `_drafts`. Projects live in `_projects`. The about page is `_pages/about.md`.

## Local build

Ruby 3.2+ and [ImageMagick](https://imagemagick.org/) (`convert`).

```bash
bundle install
bundle exec jekyll serve
```

Docker also works, via the al-folio image:

```bash
docker compose up
```

The site is then at `http://localhost:8080`.

## Deploy

Pushes to `master` run `.github/workflows/deploy.yml`, which builds the site and deploys `_site` with GitHub's Pages actions. In the repository settings, set Pages to **GitHub Actions** (not a branch).

`CNAME` stays `jovany.wang`. `url` is `https://jovany.wang` and `baseurl` is empty.
