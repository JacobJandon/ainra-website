# AINRA — website (static export)

The deployable static build of the AINRA site. **This repo is generated** from the source monorepo
([JacobJandon/ainra](https://github.com/JacobJandon/ainra), `site/` + `tools/site.sh`) — do not hand-edit
here; edit the source and re-export.

- **Live:** https://ainra.vercel.app
- **Deploy:** connect this repo to Vercel with **no build step** (Framework preset: *Other*, Build Command: empty,
  Output Directory: `.`). Every push auto-deploys.
- Fully self-contained: no CDN, no external fonts (Pixelify Sans bundled, OFL), no trackers, zero telemetry.

## Re-export (from the monorepo)
```sh
# in the JacobJandon/ainra checkout:
bash tools/export-site.sh    # rebuilds site/ and pushes it here
```
