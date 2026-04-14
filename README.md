# R & Data Visualization

**Finley Hardie — INFO 3200 · University of Denver**

Data visualization work from INFO 3200 at the Daniels College of Business. Projects cover the full range of ggplot2 chart types, geospatial mapping with real crime data, and the statistical reasoning behind each visualization — built around the Grammar of Graphics framework.

---

## Projects

### Deviation, Distribution & Correlation (`projects/w2-deviation-distribution-correlation/`)
Statistical visualization of clothing expenditure data — covering the three chart families used most in business analytics reporting.

- Histograms and density plots for price index distribution
- Correlation matrix visualization using `ggcorrplot`
- Scatter plot with smoothed trend line and linear regression model
- Formal linear regression output with `lm()` and `summary()`

**Tools:** `ggplot2` · `ggcorrplot` · `dplyr` · `broom` · `gt`

---

### Geospatial Mapping — Denver Crime Data (`projects/w3-geospatial-mapping/`)
Static and interactive maps built from a real Denver crime dataset — plotting incident locations across the metro area with drill-down to county and neighborhood level.

- Static maps using `ggplot2` + `sf` with state and county boundary overlays
- Coordinated spatial filtering to zoom into Colorado
- Interactive Leaflet map with clickable markers and popup labels showing offense category
- Crime frequency analysis with `group_by`, `summarize`, and `top_n`

**Tools:** `ggplot2` · `sf` · `leaflet` · `rnaturalearth` · `dplyr` · `maps`

---

### Bar & Line Charts — Retail Sales Analysis (`projects/w2-bar-and-line-charts/`)
Sales analysis using the Sample Superstore dataset — the go-to business dataset for practicing commercial data visualization.

- Bar charts of total sales by sub-category and category
- Faceted bar charts breaking down category sales by region
- Monthly sales trend line chart
- Multi-year sales comparison with color-coded lines by year

**Tools:** `ggplot2` · `dplyr` · `lubridate` · `forcats` · `readxl`

---

## Tools

`R` · `ggplot2` · `Leaflet` · `sf` · `dplyr` · `lubridate` · `ggcorrplot` · `rnaturalearth`

---

*University of Denver · Daniels College of Business · INFO 3200*
