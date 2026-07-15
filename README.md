# Netflix-Movies-and-TVshows-Visualization-PowerBI

This is a Power BI project that creates interactive dashboards for Netflix content visual analysis.

## Dataset
we use 2 datasets
* the first one is Netflix Movies and TV Shows on [kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows) 
* the second one is IMDb score from [IMDb Datasets](https://www.imdb.com/interfaces/) (note that we use title.basics.tsv and title.ratings.tsv)
then we combine it all together using `data_preparation.ipynb` and the final preprocessed data is in `data/netflix_titles_with_IMDB.csv`

## Results
This project depicts 2 story points.
1. an overview of Netflix content \
![page1: An overview of Netflix content](img/page1.gif "page1")

2. Top IMDB score contents \
![page2: Top IMDB score contents](img/page2.gif "page2")A

You can find it by following Power BI link below.

## Links 
[Power BI dashboard]https://kluniversityin-my.sharepoint.com/:u:/g/personal/2200039050_kluniversity_in/IQAdXsXHMxbuRIjFvlwEtO76AbK6V3XQbGa5471PCSYypg0?e=pADVJx

# 🎬 Netflix Movies & TV Shows Analytics Dashboard

An end-to-end data analytics project transforming raw, unstructured streaming catalog data into an interactive, decision-ready business intelligence solution using Power BI, Power Query, and DAX.

## 📊 Live Dashboard Preview
* **Page 1: Global Catalog Overview** (Volume, Growth, and Demographics)
* **Page 2: Content Performance & Discovery** (Audience Sentiment and Quality Metrics)

---

## 📌 Project Overview & Motivation
On the surface, public streaming catalogs appear clean and highly organized. In reality, production data is deeply unstructured. This project simulates a real-world analytics pipeline by tackling a messy public Netflix catalog and merging it with millions of rows of user sentiment data from IMDB to answer a critical business question: **Where does content volume align—or conflict—with content quality?**

### Key Challenges Solved:
* **Multi-Value Fields:** Handled single attributes (Genres, Countries) packed with comma-separated strings without duplicating the core metrics.
* **Data Schema Consolidation:** Merged disparate streaming records with external audience reaction databases (IMDB) to add multi-dimensional depth.
* **Actionable C-Suite Insights:** Transitioned raw tabular tracking into high-level visuals (Treemaps, Combo Charts, Custom NLP Word Clouds) designed for content acquisition stakeholders.

---

## 🛠️ Tech Stack & Tools
* **Data Extraction & Transformation:** Power Query (M Formula Language)
* **Data Modeling:** Relational Star Schema (Fact and Dimension framework)
* **Analytical Calculations:** Python,DAX (Data Analysis Expressions)
* **Visualization:** Power BI Desktop
* **Custom Visual Extensions:** AppSource Advanced Card, Word Cloud

---

## 🗺️ Data Pipeline & Methodology

[Raw Content Catalog + IMDB Ratings]
│
▼
[Power Query ETL] ───► (Null handling, Data type casting, String splitting)
│
▼
[Star Schema Model] ───► (Establishing Dimensions vs. Fact Tables)
│
▼
[DAX Measure Engine] ───► (Dynamic Rating Averages, Rolling Vote Counts)
│
▼
[Interactive Dashboard] ───► (Overview Canvas & Strategy Deep-Dive)

## 🚀 Key Business Insights Discovered

* **The Growth Curve Shifts:** Data surfaces an aggressive content acquisition trajectory peaking heavily in 2019, followed by an intentional structural plateau through 2021—marking a shift from absolute volume to targeted library curation.
* **Production Geography Dominance:** Content generation remains heavily asymmetrical; the United States and India alone anchor over half of the platform's overall catalog assets.
* **The Volume vs. Quality Conflict:** The genres with the highest global volume footprint (e.g., standard Comedies and massive International Packages) frequently show lower overall user satisfaction scores compared to targeted, low-volume niche categories like standalone Documentaries.