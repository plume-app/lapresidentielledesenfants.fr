# lapresidentielledesenfants.fr

Static mirror of the Framer site, hosted on GitHub Pages.

## Deployment

You can manually run the workflow from the Actions tab.

https://github.com/plume-app/lapresidentielledesenfants.fr/actions/workflows/deploy.yml

click on the "Run workflow" button and select the `master` branch.

## Scrape

```bash
FRAMER_URL=https://numerous-finance-657341.framer.app/ npm run scrape
```

Then commit `dist/` and push.

## Test locally

Serve the generated `dist/` over HTTP (don't open via `file://` — ES modules won't load):

```bash
npx serve dist
```

