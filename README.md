# mckenna.holdings

Company website for [McKenna Holdings LLC](https://mckenna.holdings). Single static page —
no framework, no build step, no external requests. All CSS is inlined in `index.html`;
icons are inline SVG; type is the system font stack.

## Layout

- `index.html` — the whole page
- `assets/favicon.svg` — favicon
- `CNAME` — custom domain for GitHub Pages (added once DNS is pointed)
- `.nojekyll` — serve files as-is, no Jekyll processing

## Local preview

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Deploy

GitHub Pages serves the `main` branch from the repository root. Pushing to `main` publishes.

## DNS

The domain is registered at Squarespace. Apex `mckenna.holdings` points at the four
GitHub Pages A records; `www` is a CNAME to `mckennasoftware.github.io`.
