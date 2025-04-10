# Krisha.kz Apartment Scraper & Analytics

This project collects real estate listings from [Krisha.kz](https://krisha.kz), cleans and structures the data, stores it in ClickHouse, and visualizes everything in Power BI. It gives you a full pipeline: from raw web pages to a sleek, interactive dashboard.

---

## What it does

- Scrapes apartment listings from Krisha.kz (multi-page support)
- Extracts detailed attributes like:
  - Price
  - Room count
  - Square meters & kitchen size
  - Year of construction
  - House type
  - Floor info (e.g., 3 out of 9)
  - Residential complex name
  - Ceiling height, parking, toilet type, etc.
- Cleans the data:
  - Removes non-numeric characters
  - Converts m² fields to numbers
  - Splits location into city & district
- Sends the cleaned data to a ClickHouse database
- Power BI dashboard connects to ClickHouse via ODBC

---

## Tech stack

- **Python** — for scraping & parsing
- **ClickHouse** — fast columnar database for analytics
- **Power BI** — to visualize everything
- **BeautifulSoup** + `requests` — for HTML parsing
- `clickhouse-connect` — Python client for ClickHouse

---

## How to use

### 1. Clone the project

git clone https://github.com/MeniskovMessi/krisha-analysis
cd krisha-analysis
