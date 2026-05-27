# Airbnb New York City 2019 — Data Analysis

A comprehensive data analysis of ~43,000 Airbnb listings across New York City's five boroughs using Power BI and Excel. The project explores room type distribution, neighbourhood dominance, host behaviour, pricing patterns, availability trends, and seasonal review patterns — delivering actionable insights for Airbnb's content strategy and traveller decision-making.

**Author:** Ashwin Suryawanshi | **Tools:** Power BI, Excel, PowerPoint

---

## Files in This Repository

| File | Description |
|------|-------------|
| `Airbnb_Data_Analysis.pbix` | Interactive Power BI dashboard — 2 pages (Overview + Analysis), 5 KPI cards, 6 charts, 1 pivot table |
| `Airbnb_NYC_2019_Detailed_Analysis.pptx` | 17-slide presentation — dataset overview, key insights, charts, and business recommendations |

---

## Tools & Technologies

- **Power BI** — KPI cards, area chart, clustered bar chart, tables, pivot matrix, date slicer
- **Excel** — Data cleaning and preprocessing
- **PowerPoint** — Insight presentation and storytelling

---

## Dataset

**Source:** Inside Airbnb — NYC 2019
**Period:** March 2011 – June 2019
**Size:** ~43,000 listings

| Column | Description |
|--------|-------------|
| `id` | Unique listing identifier |
| `name` | Listing title / property name |
| `host_id` | Unique host identifier |
| `host_name` | Name of the host |
| `neighbourhood_group` | NYC borough (Manhattan, Brooklyn, Queens, Bronx, Staten Island) |
| `neighbourhood` | Specific neighbourhood within the borough |
| `latitude` / `longitude` | Geographic coordinates of the listing |
| `room_type` | Entire home/apt, Private room, or Shared room |
| `price` | Nightly price in USD |
| `minimum_nights` | Minimum nights required per booking |
| `number_of_reviews` | Total reviews received |
| `last_review` | Date of most recent review |
| `reviews_per_month` | Average monthly review count |
| `calculated_host_listings_count` | Number of listings managed by the host |
| `availability_365` | Days available per year |

---

## Power BI Dashboard (2 Pages)

### Page 1 — Overview

| Visual | Type | Fields | Purpose |
|--------|------|--------|---------|
| Max No. of Properties Listed (Borough) | KPI Card | neighbourhood_group (min) | Top borough by listings |
| Host With Max No. of Properties Listed | KPI Card | host_name (min) | Top host name |
| Average Price | KPI Card | Sum of price | Average nightly rate across all listings |
| Property With Max No. of Reviews | KPI Card | name (min) | Most reviewed property name |
| Listings by Borough | Table | neighbourhood_group, Sum of calculated_host_listings_count | Borough-level listing count |
| Reviews by Room Type | Table | room_type, Sum of reviews_per_month | Review volume per room category |
| Availability by Room Type | Table | room_type, Sum of availability_365 | Annual availability per room category |
| Top Hosts by Listing Count | Table | host_name, Sum of calculated_host_listings_count | Host ranking by portfolio size |
| Reviews Per Month Over Time | Area Chart | Month (from last_review), Sum of reviews_per_month | Seasonal review trend |
| Most Reviewed Properties | Clustered Bar Chart | name, Sum of number_of_reviews | Top listings by total review count |

### Page 2 — Analysis

| Visual | Type | Fields | Purpose |
|--------|------|--------|---------|
| Count of Room Type | KPI Card | room_type count | Total room types |
| No. of Entire Homes / Apartments | KPI Card | room_type filter | Entire home/apt count |
| No. of Private Rooms | KPI Card | room_type filter | Private room count |
| No. of Shared Rooms | KPI Card | room_type filter | Shared room count |
| Price by Borough | Table | neighbourhood_group, Sum of price | Borough-level pricing comparison |
| Host Listings by Borough (Pivot) | Pivot Matrix | host_name (rows), neighbourhood_group (columns), Sum of listings | Cross-borough host portfolio breakdown |
| Date Slicer | Slicer | last_review date | Filter all visuals by review date range |

---

## Key Insights

| Finding | Detail |
|---------|--------|
| **Room type split** | Entire home/apt: 22,740 (~52%) · Private room: 20,220 (~46%) · Shared room: 1,074 (~2%) |
| **Borough dominance** | Manhattan: 19,875 listings · Brooklyn: 18,152 · Together = ~89% of all NYC listings |
| **Top host** | Michael — 416 listings across all 5 boroughs; commercial-scale hosting |
| **Average price** | $160.21 per night — significantly influenced by Manhattan premium pricing |
| **Seasonal peak** | Reviews peak in June (801) and July (830) · Drop below 160 from August–November |
| **Most reviewed property** | "Room near JFK Queen Bed" — ~830 reviews/month, likely in Queens near JFK Airport |
| **Availability pattern** | Entire homes and private rooms: 366 days/yr · Shared rooms: ~232 days (seasonal) |
| **Borough-specific trends** | Shared rooms rare in Manhattan · Queens has more private rooms · Staten Island least diverse |
| **Host concentration** | Sonder (commercial operator) concentrated in Manhattan · Other top hosts borough-specific |

---

## Presentation Structure (17 Slides)

| Slide | Content |
|-------|---------|
| 1 | Title — Airbnb NYC 2019 Data Analysis |
| 2 | Company Overview — Airbnb history, global presence (220+ countries, 4M+ hosts, 1B+ arrivals) |
| 3 | Project Introduction — Objectives, tools used (Power BI, Excel), dataset source |
| 4 | Dataset Overview — 43,000 listings, March 2011–June 2019, key columns |
| 5 | Room Type Distribution — Entire home 52%, Private room 46%, Shared 2% |
| 6 | Neighbourhood Group Distribution — Manhattan 19,875 · Brooklyn 18,152 |
| 7 | Room Type vs Neighbourhood — Borough-specific room type patterns |
| 8 | Host Insights — Michael (416 listings), David, Sonder, John |
| 9 | Host Presence Across Boroughs — Multi-borough vs borough-specific hosts |
| 10 | Room Availability — Entire homes 366 days · Shared rooms 232 days |
| 11 | Review Patterns Over Time — June/July peak, August–November dip |
| 12 | Reviews by Room Type — Entire home: 25,345 · Private: 22,225 · Shared: 1,156 |
| 13 | Most Reviewed Property — JFK Queen Bed, ~830/month |
| 14 | Average Pricing — $160.21 NYC average |
| 15 | Summary of Key Insights |
| 16 | Recommendations — Airbnb strategy + traveller tips |
| 17 | Thank You |

---

## Business Recommendations

**For Airbnb:**
- Boost marketing campaigns in summer (June–July) — peak review and booking season
- Focus growth efforts in Queens and the Bronx — underpenetrated relative to Manhattan/Brooklyn
- Monitor commercial-scale hosts (Michael, Sonder) — 400+ listings per host signals hotel-like operations

**For Travellers:**
- Consider private rooms in outer boroughs (Queens, Brooklyn) for better value vs Manhattan
- Book in advance for June–July peak season — highest demand period
- Properties near JFK Airport (Queens) show the highest review engagement — strong guest satisfaction signal

---

## Topics

`power-bi` `airbnb` `nyc` `new-york` `eda` `data-analysis` `real-estate` `excel` `tourism` `kpi-dashboard`
