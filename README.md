# Amazon Prime Video — Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)
![Competition](https://img.shields.io/badge/NASCON-Data%20Analytics-orange)

An interactive **Power BI** dashboard that explores Amazon Prime Video's title catalog — breaking down the library by type, genre, content rating, country, and release year. Built as a competition entry for **NASCON**, FAST NUCES' largest tech competition.

---

## Dashboard Preview

![Amazon Prime Dashboard](images/dashboard.jpeg)

> _Add your exported screenshot as `images/dashboard.png` (create an `images/` folder in the repo and drop it in), then delete this line._

---

## What It Shows

A single interactive page with 12 visuals answering the core "what's in the catalog?" questions:

| Visual | Question it answers |
|---|---|
| **KPI cards** | Total Titles, Total Genres, Total Ratings, Total Directors at a glance |
| **Movies vs. TV Shows** (donut) | How the catalog splits between the two content types |
| **Titles by Country** (filled map) | Which countries contribute the most content |
| **Titles by Release Year** (area chart) | How the catalog has grown over time |
| **Ratings by Total Shows** (bar) | Distribution across content-rating categories |
| **Genres by Total Shows** (bar) | The most common genres in the library |
| **Start / End Date** (slicers) | Filter the whole report by release-year range |

Every visual cross-filters the others, so selecting a country, genre, or year instantly reslices the entire page.

---

## Dataset

Built on the **`amazon_prime_titles`** dataset — Amazon Prime Video's public catalog of movies and TV shows. Key fields used:

- `type` — Movie or TV Show
- `title`, `director`
- `country` — production country
- `release_year`
- `rating` — content rating (e.g., PG-13, R, TV-MA)
- `listed_in` — genre categories

The data was cleaned and shaped in **Power Query** (handling multi-value genre/country fields and missing entries) before modeling.

---

## Skills Demonstrated

- **Power BI Desktop** — report design and interactive dashboard layout
- **Power Query (M)** — data cleaning, splitting multi-value columns, handling nulls
- **DAX** — measures for the KPI cards and aggregations
- **Data visualization** — choosing the right chart per question and designing a single-glance layout
- **Cross-filtering & slicers** — interactive exploration by year, genre, country, and type

---

## How to Open

1. Install **[Power BI Desktop](https://powerbi.microsoft.com/desktop/)** (free, Windows).
2. Download `Amazon_Prime_Dashboard.pbix` from this repo.
3. Open it in Power BI Desktop — the dataset is embedded, so it loads with no extra setup.



