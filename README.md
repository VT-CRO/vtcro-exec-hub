# VT CRO Exec Hub

Internal reference site for VT CRO executives: purchasing steps, lab access, quick-copy fund numbers, and the constitution.

It's a static site (`index.html` + `assets/`) with no build step.

## Hosting (Vercel)

Import this repo in Vercel with the framework preset set to **Other**, and leave the build command and output directory empty. Every push to `main` redeploys.

The page has a `noindex` tag and `robots.txt` blocks crawlers, but the URL itself is not password protected.

## Editing

- **Add a section:** copy a `<section class="page">` block in `index.html` and give it a unique `id`, `data-title` and `data-group`. The sidebar, search and routing pick it up automatically.
- **Change a link:** all URLs are in the `LINKS` object near the bottom of `index.html`.
- **Teams** for the purchase-order note are in `TEAMS`, right below `LINKS`.
- See the comment at the top of `index.html` for the reusable building blocks.

A private mirror also exists on claude.ai: https://claude.ai/artifact/WyBioDs3XKh3C5TuzDy6BN. To update it, publish the page *without* the `<!doctype>`/`<html>`/`<head>`/`<body>` wrapper.
