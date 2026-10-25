# blog

A Jekyll blog (minima theme), deployed to GitHub Pages via GitHub Actions.

## Write a post

Add `_posts/YYYY-MM-DD-title.md` with front matter:

```yaml
---
layout: post
title: "My Post"
---
```

## Preview locally (Docker)

```sh
docker run --rm -it -v "$PWD":/srv/jekyll -p 4000:4000 ruby:3.3 \
  bash -c "cd /srv/jekyll && bundle install && bundle exec jekyll serve --host 0.0.0.0 --livereload"
```

Then open http://localhost:4000/
