# Dor0r0 Blog

GitHub Pages project site based on Jekyll.

Expected URL:

- `https://kjs36202.github.io/Dor0r0.github.io/`

## Local development

Recommended Ruby version:

- `3.3.0`

Commands:

```bash
/Users/Dor0r0/.rubies/ruby-3.3.0/bin/bundle install
/Users/Dor0r0/.rubies/ruby-3.3.0/bin/bundle exec jekyll serve
```

Then open:

- `http://127.0.0.1:4000/Dor0r0.github.io/`

## Deployment

This repository includes a GitHub Actions workflow for Pages deployment.

On GitHub, set:

1. `Settings`
2. `Pages`
3. `Source: GitHub Actions`

After pushing to `main`, the site should deploy automatically.

## Switching To A User Site

If you later rename the repository to `kjs36202.github.io`, update `_config.yml` like this:

```yml
url: "https://kjs36202.github.io"
baseurl: ""
```
