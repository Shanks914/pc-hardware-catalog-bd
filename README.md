# PC Hardware Catalog — Bangladesh (BDT)

This repository is the data feed for the PC Hardware Analyzer JavaFX app. `catalog.json` is fetched at startup and through the app's Sync action.

## Catalog format

The feed uses `schemaVersion: 1`, `currency: BDT`, and a `components` array. Each record contains a stable ID, component name/type, BDT price, source article URL, Wikipedia revision ID, and source USD value.

## Sources and conversion

The catalog is compiled from Wikipedia CPU and GPU price tables. Each entry links to its source article and revision. The source USD amount is retained as `sourcePriceUsd`; `priceBdt` is calculated using Bangladesh Bank's September 24, 2026 reference rate of 123.1754 BDT per USD. The rate source is https://www.bb.org.bd/en/index.php/econdata/rfrexrate.

Wikipedia content is reused under CC BY-SA 4.0. Article URLs and revision IDs are included for attribution; this catalog and modifications are released under the same share-alike terms. The listed values are Wikipedia's published prices converted to BDT, not local retailer quotes.
