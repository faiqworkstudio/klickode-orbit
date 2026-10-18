# Klickode Orbit

**Own a planet. Build a world inside.** Orbit is a shared universe of 9,999 Genesis planets. People design a planet (name, colours, ring, moon, crystals), claim its number, write a small world inside it (a dedication and three chapters), and get a certificate of ownership with a fingerprint code and a generated seal. Anyone can search the universe by planet name, number or owner.

| File | What it is |
|---|---|
| `index.html` | The Orbit site: 3D flight, planet designer with live pricing, galaxy map and search, planet sheet (world inside + certificate), how it works, FAQ and brand star systems. |
| `plan.html` | Orbit strategy: product, why it sells, occasions calendar, price ladder and lucky numbers, revenue model, marketing, role in the Klickode portfolio, roadmap, risks and KPIs. |
| `original.html` | The original concept page, kept for reference. |

## Registry storage

When published as a claude.ai artifact, claims are shared between visitors through the artifact database:

- `claims/<number>`: `{owner, at}`. The lock that makes one number belong to one owner (claimed with a short lease).
- `worlds/<user id>`: `{planets: {<number>: planet}}`. Each person writes only their own document; everyone reads all of them.

Opened anywhere else, the page keeps planets in the browser's local storage so the full flow still works. Payments are not wired up: claiming is free in this preview.

`index.html` is written as an artifact body (no `<html>/<head>` wrapper). To self-host it, wrap it in a standard document shell. Both pages load three.js r128 and Google Fonts from public CDNs.
