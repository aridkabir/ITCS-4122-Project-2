# Video Game Sales Analysis

An exploration of what factors most influence global and regional video-game sales, particularly game genre, platform, publisher, and region.

---

## Project Overview

**Question:**  
What factors influence video-game sales the most across global and regional markets?

**Why:**  
Video games have always been something that I’ve enjoyed, and I’ve always wondered why certain games become global hits while others only succeed in specific regions. With so many genres, platforms, and publishers, this dataset gives a great opportunity to understand what drives sales.

**Key factors examined:**
- **Genre** (e.g., Action, Shooter, Role-Playing, etc)  
- **Platform** (e.g., Wii, PS3, DS, etc)  
- **Publisher**  
- **Regional Sales** (North America, Europe, Japan)  
These are the big factors that I wanted to explore in this project, seeing how each one directly plays into sales figures.
---
**Target Audience**

This dashboard is designed for:

Gamers, who are curious about metrics throughout history

Developers, looking to see what games are most popular worldwide

Marketing teams, who determine which regions respond best to certain types of games

Students, studying the gaming industry


## Dataset Description

- **Source:** Kaggle — Video Game Sales with Ratings  
- **Rows:** ~ 16,500 game entries  
- **Columns used:**  
  - `Name` — title of the game  
  - `Genre` — game’s category  
  - `Platform` — console it was released on  
  - `Publisher` — company that published the game  
  - `Year` — release year  
  - `Global_Sales` — worldwide sales (millions)  
  - `NA_Sales`, `EU_Sales`, `JP_Sales` — regional sales (millions)
 
  I picked this dataset specifically because of the wide variety of items, spanning from the 1980's to 2020.
  This gives us a lot of items to work with, and allows us to see trend data very easily utilizing PowerBI.

---

## Preprocessing / Cleaning

Here are some steps taken to make the data analysis reliable:

1. **Remove missingness:** rows with missing Genre, Platform, Publisher, or Sales fields were removed to make cards and visuals cleaner.  
2. **Drop zero-sales entries:** games with 0 sales in all regions were removed.  
3. **Standardize categories:** ensured consistent formatting for platforms and publishers.  

---

## Visualizations / Design Choices

| Chart | Purpose | Design / Reasoning |
|-------|---------|----------------------|
| **Top-Selling Games** (Horizontal Bar) | Shows which titles sold the most worldwide | Horizontal layout makes long game titles readable |
| **Regional Sales by Genre** (Grouped Bar) | Highlights how NA, EU, and JP differ in game preferences | Grouped bars allow easy side-by-side comparison |
| **Sales by Platform / Genre / Publisher** (Dashboard Filters) | Helps explore specific segments of the market | Filters make exploring subcategories simple |
| **Game Detail Panel** (KPI Cards) | Shows release year, platform, publisher, and sales for selected game | Updates dynamically and gives focused context |

**Color / Layout Choices:**
- Distinct colors for NA (yellow), EU (blue), and JP (red) to keep regional comparisons clear  
- Neutral, readable palette for ranking chart  
- Dashboard layout organized for natural top-down analysis flow (overview → detail)

---

## Reflection

**What worked well:**
- Filters made it easy to explore the dataset across platform, genre, and publisher  
- Regional comparison chart clearly showed how preferences differ across markets  
- KPI detail cards gave helpful context for each selected game  
- Top-seller ranking chart immediately highlighted standout titles

**What was challenging / didn’t work as planned:**
- Getting all visuals to properly sync with filters was tricky  
- Genre/region bar chart becomes crowded with too many categories  
- Sparse data for some publishers limited comparison  
- Lack of time-series data restricted long-term trend analysis

**If I had more time, I’d…**
- Add time-series visualizations for platform/genre popularity over the years  
- Improve the visual aesthetics and spacing of the dashboard  
- Work a way to show thousands as thousands and millions as millions
- Incorporate critic/user rating data to compare sales vs. quality  
- Add geographic mapping when selecting region

## References
- Kaggle Dataset: Video Game Sales with Ratings — https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings
- Microsoft PowerBI — https://www.microsoft.com/en-us/power-platform/products/power-bi
- ChatGPT — Layout / Formatting Assistance

[Dashboard](https://app.powerbi.com/reportEmbed?reportId=cb1c1178-1d15-4926-b2f8-5befae168b69&autoAuth=true&ctid=88d59d7d-aecb-41b2-90c5-55595de02536)
