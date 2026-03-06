# PySpark IMDB Data Analysis

## Overview

This project demonstrates **end-to-end large-scale data analysis in PySpark** on **AWS EMR**, using a multi-table IMDB dataset stored in **AWS S3**. I used the **Spark DataFrame API** to ingest, clean, join, transform, and analyze **50M+ records across 4 datasets**, then answered targeted analytical questions about movies, actors, genres, ratings, runtimes, and title categories.

- Work with **distributed data at scale**
- Use **PySpark joins, filters, explode, split, casting, groupBy, aggregations, sorting, and multi-step query pipelines**
- Turn messy raw data into **clear analytical outputs and visual summaries**


---

## Dataset Scale

| Table | Rows | Columns |
|---|---:|---:|
| `name.basics` | 9,706,922 | 6 |
| `title.basics` | 6,321,302 | 9 |
| `title.principals` | 36,468,817 | 6 |
| `title.ratings` | 993,153 | 3 |

**Total records processed:** 53M+

---
## Highlights
### Distributed aggregations and ranking
Used Spark to compute:
- number of distinct genres
- average rating by genre
- most common job categories in title principals
- top genres by shortest average runtime
- yearly movie counts for specific actors

### Multi-table analytical querying
Joined people, titles, principals, and ratings to answer targeted questions such as:
- movies featuring both Johnny Depp and Helena Bonham Carter
- Brad Pitt movies released after 2010
- Zendaya movie counts by year
- 2019 movies with ratings above 9.7
- whether Clint Eastwood or Harrison Ford has the higher average rating
- highest-rated Chris Evans movies
- percentage of adult titles involving actors vs actresses
- most common character names in Romance movies

---

## Tech Stack

- **PySpark**
- **Spark DataFrame API**
- **Python**
- **Pandas**
- **Matplotlib / Seaborn**
- **Amazon S3**
- **Amazon EMR**
- **Jupyter Notebook**

---

## Repository Contents

- `PySpark_IMDB_Data_Analysis.ipynb` — full notebook with ingestion, transformations, analysis, and visualization
