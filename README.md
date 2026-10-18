# Klickode Orbit

The cinematic line of Klickode Studio: 3D scroll websites people fly through. Customers move inward through orbits: **Outer** (Orbit Lite and Kit), **Inner** (Orbit Launch, 14 days), **Stay in orbit** (Care), and the **Core** (Klickode Studio work). Every project is a mission (`ORB-001`…) in the Mission log.

| File | What it is |
|---|---|
| `index.html` | The Orbit site: WebGL flight, live planet builder, Mission log of four concept missions, orbit pricing, and a mission-brief composer with lift-off dates. |
| `plan.html` | Orbit strategy: role in the Klickode portfolio, the orbit/gravity model, name system, portfolio playbook, market, revenue model, marketing cadence, roadmap, risks and KPIs. |
| `original.html` | The original concept page, kept for reference. |

`index.html` is written as an artifact body (no `<html>/<head>` wrapper). To self-host it, wrap it in a standard
`<!doctype html><html><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1"></head><body>…</body></html>`.
Both pages load three.js r128 and Google Fonts from public CDNs.
