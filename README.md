# hco-splendid-supplier-data

Supplier source files for Splendid Trading's Intelligent Products deployment (`splendid`),
read by its Loader from the addresses on `IP Settings: Suppliers` in the SPLENDID Confluence space.

| Supplier | File | Ticket |
| --- | --- | --- |
| Artis UK | `artis/artis-slice-15.csv` | HCP-243 thin slice |

`artis-slice-15.csv`: 15 real Artis UK products (5 Tableware, 5 Cutlery, 5 Barware), taken read-only
from the legacy Splendid export (HCP-248, `raw_` layer of splendid-trading.db), in the Artis XLSX
column names (Part, Description, Brand, Category, List Price, Web URL) plus the scraped product image
(Image). List Price is Artis's public list price in pounds, written with a `£` so the currency is
carried. Net cost per piece is never included (Splendid Standing Rule 3.1).
