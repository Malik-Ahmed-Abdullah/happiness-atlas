# happiness-atlas 🌍

An interactive data visualization dashboard exploring the **World Happiness Report 2019** — 156 countries, 7 wellbeing indicators, and 7 distinct interaction types built with D3.js.

**[Live Demo →](https://YOUR-USERNAME.github.io/happiness-atlas/)**

---

## About the Dataset

The [World Happiness Report](https://worldhappiness.report/) ranks countries by how happy their citizens perceive themselves to be, measured via the Cantril ladder (0–10 scale). The 2019 edition covers **156 countries** with the following attributes:

| Field | Description |
|---|---|
| `score` | Overall happiness score (Cantril ladder, 0–10) |
| `gdp` | GDP per capita (log scale) |
| `social` | Social support index |
| `health` | Healthy life expectancy |
| `freedom` | Freedom to make life choices |
| `generosity` | Generosity index |
| `corruption` | Perceptions of government corruption |

---

## Interaction Types

All 7 interaction types from Shneiderman's visual information-seeking mantra are implemented:

| # | Type | Implementation |
|---|---|---|
| 1 | **Select** | Click any scatter plot point to select a country and view its detailed stats |
| 2 | **Filter** | Region dropdown filters all three chart panels simultaneously |
| 3 | **Encode** | Toggle color encoding between Region, Happiness Score, and GDP per Capita |
| 4 | **Connect** | Hovering a point in the scatter plot highlights the same country in the parallel coordinates |
| 5 | **Reconfigure** | Y-axis dropdown switches the ranking metric across the bar chart |
| 6 | **Elaborate** | Hovering a line in the parallel coordinates reveals a detailed tooltip with all 7 indicators |
| 7 | **Abstract** | The Top-N slider adjusts how many countries are shown (5–30), zooming in or out on the data |

---

## Visualizations

### Scatter Plot — Happiness vs GDP
Shows the relationship between economic output and reported happiness. Points are colored by the selected encoding. Click to select, hover to connect with the parallel coordinates view.

### Bar Chart — Country Rankings
Ranks the top N countries by the chosen metric. Updates live with filter and reconfigure controls.

### Parallel Coordinates — Multi-Dimensional Profiles
Plots each country as a line across all 7 axes simultaneously, revealing trade-offs and patterns across indicators.

---

## Tech Stack

- **D3.js v7** — all charts and interactions
- **Vanilla HTML/CSS/JS** — zero build tools, no frameworks
- **Google Fonts** — DM Serif Display + DM Sans

---

## Running Locally

No build step needed — just open the file:

```bash
git clone https://github.com/YOUR-USERNAME/happiness-atlas.git
cd happiness-atlas
open index.html  # or just double-click it
```

---

## License

Data: [World Happiness Report](https://worldhappiness.report/) / Gallup World Poll.  
Code: MIT

