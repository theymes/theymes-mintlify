# Documentation project instructions

This is the Theymes documentation site on [Mintlify](https://mintlify.com). Pages are MDX with YAML frontmatter. Site config lives in `docs.json`.

Published at docs.theymes.com. The legacy developer site at developers.theymes.com is still Docusaurus in the main Theymes repo (`services/dev-docs`) until cutover.

## About this project

Theymes is customer support software for gaming companies. This site will hold **all** public docs:

- `product/` — product/help docs for support teams using the agent desktop
- `developers/` — integration docs (SDK, player metadata, automation, API overview)
- API reference tab — OpenAPI from `https://api.theymes.com/openapi`

## Structure

- Product pages go in `product/`. Do not nest them under `developers/`.
- Developer pages go in `developers/`. SDK pages live in `developers/sdk/{unity,ios,android,web}/`.
- Register every new page in `docs.json` navigation. Product content uses the Product tab; integration content uses the Developers tab.
- The API reference tab is generated from OpenAPI. Auth and overview prose stays in `developers/api.mdx`.

## Terminology

- Use **player**, not user, for people playing the game
- Use **agent** for support staff in the Theymes app
- Use **help center** for the in-game / widget support UI
- Use **Theymes SDK** (not “TheymesSdk” except in code)

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Mintlify callouts: `<Tip>`, `<Info>`, `<Warning>` (not Docusaurus `:::tip`)
- Mintlify tabs: `<Tabs><Tab title="Swift">` (not `@theme/Tabs`)

## Content boundaries

- Do not document internal admin-only Theymes features
- Do not publish draft SDK pages (for example retention tracking) unless they are ready
- Android SDK docs may stay as a stub until the native docs exist
