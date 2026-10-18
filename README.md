# Klickode Orbit

Cinematic 3D scroll websites, sold three ways: **Orbit Kit** (template), **Orbit Launch** (done-for-you, 14 days) and **Orbit Care** (monthly).

| File | What it is |
|---|---|
| `index.html` | The Orbit product site: a WebGL flight with a live "build your planet" configurator, process chapters, pricing and contact. |
| `plan.html` | Year-one business plan: idea, market, customers, pricing, an adjustable revenue model, marketing, roadmap, risks and KPIs. |
| `original.html` | The original concept page, kept for reference. |

`index.html` is written as an artifact body (no `<html>/<head>` wrapper). To self-host it, wrap it in a standard
`<!doctype html><html><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1"></head><body>…</body></html>`.
Both pages load three.js r128 and Google Fonts from public CDNs.
