# Klickode Orbit

**Give your company a world.** Orbit is a universe of companies. A company claims a numbered planet in the Genesis galaxy and builds an animated world inside it: hero, numbers, story, services, a quote and contacts, in its own colours, headline type and sky. Visitors explore the galaxy, warp into a planet and land in that company's world. Each company can upload its logo, which becomes a lit 3D emblem (coin, tile or diamond; enamel, brushed metal, gold or matte). Every world comes with a share kit: world link, QR code, a 3D business card with print-ready front and back (3.5 × 2 in at 300 dpi), a contact file (.vcf), a launch post image and a numbered certificate. Plans: Outpost ฿390/month, Orbit ฿990/month, Flagship ฿24,900 build + ฿990/month, and brand systems by quote.

| File | What it is |
|---|---|
| `index.html` | The Orbit site: 3D flight, six-step world builder with live preview and plan logic, galaxy map and company search, the animated world inside each planet, certificate, plans and FAQ. Includes Klickode Studio as planet No. 0001 and three labelled example worlds. |
| `plan.html` | Orbit strategy: product, value comparison, customers, price ladder, subscription revenue model with cancellations, marketing, role in the Klickode portfolio, roadmap, risks and KPIs. |
| `original.html` | The original concept page, kept for reference. |

## Registry storage

When published as a claude.ai artifact, worlds are shared between visitors through the artifact database:

- `claims/<number>`: `{owner, at}`. The lock that gives one number to one company (claimed with a short lease).
- `worlds/<user id>`: `{companies: {<number>: world}}`. Each person writes only their own document; everyone reads all of them.

Opened anywhere else, the page keeps worlds in the browser's local storage so the whole flow still works. Payments are not wired up: launching is free in this preview.

`index.html` is written as an artifact body (no `<html>/<head>` wrapper). To self-host it, wrap it in a standard document shell. Both pages load three.js r128, qrcode-generator 1.4.4 and Google Fonts from public CDNs.
