# SupplyDirect Demo: Mock Ariba-Style Sonic Radar Catalog

This is a public static mock procurement website for AI Agent / GEO retrieval testing.

It contains:

- `index.html`: SAP UI5 / OpenUI5 search homepage
- `ariba-sonic-radar.html`: intent landing page for "I want to purchase a sonic radar product on Ariba"
- `sonic-radar-procurement-catalog.html`: detailed fictional catalog file information
- `robots.txt`: crawler access rules
- `sitemap.xml`: page discovery file
- `llms.txt`: AI-oriented page index

## Disclosure

This is **not** an official SAP Ariba website. All product, supplier, pricing, and catalog data are fictional.

## GEO Research Note

This site is one of multiple mock procurement sites used in a GEO (Generative Engine Optimization)
research experiment. All sites carry the same product (SR-9000 Industrial Sonic Radar), but differ
in brand identity and supplier name, simulating competing vendors. The goal is to observe how
different GEO optimization strategies affect AI search answer rankings.

| Site | Supplier | GEO Strategy |
|------|----------|--------------|
| Mock-Ariba-Business-Network-Search | AcoustiWave Technologies Ltd. | Reference baseline |
| Mock-SupplyDirect-SonicRadar (this) | SonoCore Industrial Ltd. | Baseline (same structure) |

## Local development

```bash
npm install
npm run start
```

Open:

```text
http://localhost:8081/
```

You can also use Python:

```bash
python3 -m http.server 8081
```

## Before publishing

Replace every `https://YOUR_DOMAIN` placeholder in these files:

- `index.html`
- `ariba-sonic-radar.html`
- `sonic-radar-procurement-catalog.html`
- `robots.txt`
- `sitemap.xml`
- `llms.txt`

Example (GitHub Pages):

```text
https://your-name.github.io/Mock-SupplyDirect-SonicRadar
```

or (Vercel):

```text
https://supplydirect-geo-demo.vercel.app
```

## Test queries

- I want to purchase a sonic radar product on Ariba.
- 我想要在 Ariba 上采购一个声波雷达产品。
- Find an Ariba-style sonic radar procurement catalog.
- What is the supplier and price of the SR-9000 Industrial Sonic Radar?
- What is the MOQ and lead time of the SR-9000 Industrial Sonic Radar?
