# OperFi Developer Portal

Public API documentation for the OperFi Partner API, served at
**https://developers.operfi.com** via GitHub Pages.

## Contents

- `index.html` — renders the API reference with [Redoc](https://github.com/Redocly/redoc).
- `openapi.yaml` — the OpenAPI 3 contract. **This is a published copy.** The
  source of truth lives in the `operfi-broker-api` repo at `docs/api/openapi.yaml`,
  next to the code that implements it. When the contract changes there, the new
  version is copied here and pushed.
- `CNAME` — tells GitHub Pages to serve this repo at `developers.operfi.com`.

## How it deploys

GitHub Pages serves the repo root on the `main` branch. Any push to `main`
republishes the site within a minute or so. No build step.

## Updating the contract

Do not hand-edit `openapi.yaml` here. Edit it in `operfi-broker-api`, then copy
the updated file into this repo and push.
