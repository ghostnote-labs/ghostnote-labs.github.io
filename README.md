# Ghostnote Labs

Studio site at **https://ghostnotelabs.studio**.

Also hosts public privacy policy (`/privacy`) and terms of service (`/terms`) for Ghostnote Labs LLC products.

## Local dev

GitHub Pages builds from `main` automatically — you don't need to run Jekyll locally unless you want a preview. If you do:

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```

## Publishing

Any push to `main` rebuilds the site. See CLAUDE.md for:

- Brand / entity details
- Trademark-caution rules (why product names are stripped before publishing here)
- The strip-before-publish workflow for pulling updated legal docs from the private product repo
- Visual + voice guidelines
