# PC Hardware Catalog — Bangladesh (BDT)

This repository is the data feed for the PC Hardware Analyzer JavaFX app. `catalog.json` is fetched at startup and through the app's Sync action.

## Catalog format

The feed uses `schemaVersion: 1`, `currency: BDT`, and a `components` array. Every listing must carry a stable unique `id`, `type`, `name`, `priceBdt`, `currency`, `updatedAt` (ISO 8601), and `source` (authorized retailer/feed URL). Optional fields include `brand`, `socket`, `tdp`, and `specs`.

## Price sourcing

Only add prices from sources whose terms permit reuse and redistribution. Keep the source URL and observation time on every record. Refresh prices from the authorized source and remove discontinued listings. Do not copy another catalog's listings or present estimates as current prices.

The initial `catalog.json` is intentionally empty until a permitted source is connected. The 5,000+ current-price target requires an authorized data feed.
