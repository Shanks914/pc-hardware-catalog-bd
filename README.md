# PC Hardware Catalog — Bangladesh (BDT)

This repository is the data feed for the PC Hardware Analyzer JavaFX app. The app fetches `catalog.json` at startup and through its Sync action.

## Component coverage

| Type | Entries |
| --- | ---: |
| CPU | 1,757 |
| GPU | 359 |
| Motherboard | 100 |
| RAM | 100 |
| Storage | 100 |
| PSU | 100 |

The motherboard, RAM, storage, and PSU entries are illustrative demo records added to support the full PC-build workflow. They provide representative model/spec combinations and estimated BDT prices; they are **not verified Bangladesh retailer listings**. These records have `isDemoEntry: true` and `priceIsEstimate: true`. Verify the exact SKU, specifications, compatibility, and current local price before relying on a demo entry.

## Catalog format

The feed uses `schemaVersion: 1`, `currency: BDT`, and a `components` array. Every component includes an ID, type, name, BDT price, update timestamp, and source URL. Optional fields include brand, specifications, and compatibility details such as CPU socket.

## Sources, prices, and attribution

CPU and GPU records retain source article URLs and Wikipedia revision IDs. Their published USD price values are converted to BDT using Bangladesh Bank's September 24, 2026 reference rate of 123.1754 BDT per USD: https://www.bb.org.bd/en/index.php/econdata/rfrexrate. Wikipedia-derived content is reused under CC BY-SA 4.0; the source URLs and revision IDs provide attribution.

For illustrative motherboard, RAM, storage, and PSU entries, the `source` points to a manufacturer's product overview. It is not a price citation. Their BDT prices are estimates for demonstration only, not sourced retailer quotes.

The catalog includes Wikipedia-derived material under CC BY-SA 4.0, so the combined catalog and modifications are released under the same share-alike terms. Product and company names remain the property of their respective owners.

