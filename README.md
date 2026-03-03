# Data Science Projects — Web Scraping

A collection of **Jupyter Notebooks** for web scraping projects. The main focus is scraping multi-table data from the web (including Wikipedia) and exporting 16 structured CSV files.

---

## Table of Contents

- [Overview](#overview)
- [Notebooks](#notebooks)
- [Scraped Data](#scraped-data)
- [Tech Stack](#tech-stack)
- [Setup & Running](#setup--running)

---

## Overview

This repository contains data science work centered on web scraping using Python. The main notebook scrapes structured table data from websites and exports the results as multiple CSV files. A second notebook specifically targets Wikipedia table extraction.

---

## Notebooks

| Notebook | Size | Description |
|---|---|---|
| `dataScience_scrapping.ipynb` | 218KB | Main scraping notebook — reads HTML tables from web pages, cleans and exports data |
| `wikipedia_table.ipynb` | — | Wikipedia-specific table scraper using `pd.read_html()` or BeautifulSoup |

---

## Scraped Data

The scraping output is stored in 16 CSV files:

| File | Description |
|---|---|
| `table_1.csv` | Scraped table 1 |
| `table_2.csv` | Scraped table 2 |
| `...` | |
| `table_16.csv` | Scraped table 16 |

Each file corresponds to an individual table scraped from a source web page.

---

## Tech Stack

| Component | Technology |
|---|---|
| Notebooks | Jupyter (.ipynb) |
| Web Scraping | requests, BeautifulSoup, pandas (`read_html`) |
| Data Processing | Pandas, NumPy |
| Output | CSV files (table_1–16.csv) |

---

## Setup & Running

```bash
git clone https://github.com/jaideepj2004/data-science-projects.git
cd data-science-projects
pip install requests beautifulsoup4 pandas lxml jupyter
jupyter notebook
```

Run `dataScience_scrapping.ipynb` or `wikipedia_table.ipynb` to reproduce the scraped CSV files.
