# US Power Projection — Post-WW2 Analysis Dashboard

An interactive, single-file HTML dashboard covering US military spending, foreign aid, overseas basing costs, personnel casualties, and global engagement since 1945 — all figures inflation-adjusted to constant 2024 USD.

## Open

Open `us-military-dashboard.html` in any modern browser. No server, build step, or internet connection required beyond loading map tiles and fonts on first use.

---

## Tabs

| Tab | What it shows |
|---|---|
| **Overview** | Defense vs. foreign aid trend, KIA by conflict, spending ratios |
| **Spending** | Annual defense budget — toggle between $ billions, % of GDP, % of federal budget |
| **US Engagement** | All countries receiving US money (grants + basing), filterable by year/range |
| **Timeline** | 23 clickable events 1947–2024 — conflicts, aid programs, terror attacks |
| **Global Map** | ~60 markers: bases, access agreements, aid operations, FMS-only recipients |
| **Casualties** | Military KIA by conflict, cause of death, domestic & overseas terror deaths |
| **Foreign Aid** | Unified table — military grants vs. civilian aid vs. FMS commercial sales |
| **Compare** | Side-by-side country comparison with overlaid historical charts |
| **Sources** | Full citation index (S1–S22) with links; every stat is source-tagged |

---

## Key Features

- **Inflation adjustment** — all historical figures deflated via BLS CPI-U to 2024 USD; $1 in 1950 = $12.80 today
- **Grants vs. FMS** — distinguishes US taxpayer-funded grants (Israel, Egypt, Jordan) from commercial arms sales where the recipient pays (Saudi Arabia, Taiwan)
- **Year selector** — drag a slider or pick a quick-select year (1950–2024) on the Engagement table; range mode shows cumulative totals
- **Sortable columns** — click any column header to sort ▼/▲
- **Country source links** — each row includes direct links to USAID Explorer, CRS reports, DoD/military commands, and live trackers
- **Per-unit spending** — defense trajectory in Per Capita / Per Taxpayer / Per Soldier / Total $ modes
- **Country comparison** — select any two countries for a side-by-side bar chart, composition donut, historical overlay, and metrics table

---

## Data Sources

All data is open-source. Key sources (full citations in the Sources tab):

- **S3** — SIPRI Military Expenditure Database
- **S4** — OMB Historical Tables (White House)
- **S5** — Watson Institute Costs of War (Brown University)
- **S7/S8** — DMDC Military Casualty Statistics / CRS RL32492
- **S10** — USAID Foreign Aid Explorer
- **S11** — DoD Defense Security Cooperation Agency (DSCA)
- **S20** — RAND / Overseas Basing Commission Report
- **S21** — Congressional Budget Office — Host Nation Support
- **S22** — BLS CPI-U (inflation deflator)

---

## Libraries Used (loaded from CDN)

- [Chart.js 4.4](https://www.chartjs.org/) — all charts
- [Leaflet 1.9.4](https://leafletjs.com/) — interactive world map
- [OpenStreetMap](https://www.openstreetmap.org/) — map tiles
- Google Fonts — Bebas Neue, IBM Plex Mono, Barlow Condensed

---

## Notes

- Map tiles require an internet connection on first load; the rest runs fully offline
- All monetary figures are estimates based on publicly available data; exact figures may vary by source and methodology
- FMS (Foreign Military Sales) figures represent commercial transactions where the recipient country pays full market price — they are excluded from "aid" totals by default
