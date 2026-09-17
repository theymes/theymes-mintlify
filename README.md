# Theymes documentation

This is the documentation site for Theymes, built with [Mintlify](https://mintlify.com). It is published at [docs.theymes.com](https://docs.theymes.com).

## Structure

- `product/` — product and help-center docs (growing)
- `developers/` — SDK, player metadata, automation, and API overview
- `docs.json` — site name, branding, and navigation (Product, Developers, API reference tabs)

Do not put product docs under `developers/`. Keep SDK pages under `developers/sdk/{unity,ios,android,web}/`.

## Local preview

```bash
npm i -g mint
mint dev
```

Preview at `http://localhost:3000`.

If a page 404s, confirm you ran `mint dev` from the directory that contains `docs.json`.

## Publishing

Install the Mintlify GitHub app from the [Mintlify dashboard](https://dashboard.mintlify.com/settings/organization/github-app). Pushes to the default branch deploy automatically.
