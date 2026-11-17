# Food O'Cork

Interactive Cork City food and price atlas with a 3D map, restaurant and café directory, indicative menu prices, and proximity to major landmarks and transport hubs.

## Website

**GitHub Pages:** https://leon-bishop.github.io/Food-O-Cork/

The complete website is in [index.html](index.html). Its venue and landmark snapshot is embedded in the HTML, so GitHub Pages can serve it without a backend or separate JSON request. Internet access is required for map tiles and MapLibre assets.

## Research files

- [Venue records](data/venues.csv) — 150 initial restaurant and café listings
- [Landmarks](data/landmarks.csv) — 11 transport hubs and landmarks
- [Proximity matrix](data/proximity_matrix.csv) — preliminary proximity estimates
- [Geographic coverage gaps](research/verification/geographic_coverage_gaps.csv)
- [Venue verification queue](research/verification/venue_verification_queue.csv)

## Publish with GitHub Pages

Go to **Settings → Pages → Build and deployment → Source: GitHub Actions**. The workflow in `.github/workflows/pages.yml` deploys from `main`.

## Data quality

**Research prototype, not a verified business directory.** Many venue locations use locality proxy coordinates. The walking-minute estimates are indicative calculations, **not** pedestrian-route results. Venue trading status and current prices must be checked independently before treating them as confirmed.
