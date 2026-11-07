# Advance Book Scraping

A menu-driven Python script that scrapes book data from [books.toscrape.com](https://books.toscrape.com), a practice website made for scraping. The data there is fake demo data, not real store prices.

## What it does

1. Scrape: you enter how many listing pages to scrape. For each book it collects title, price, availability, star rating, category and description, then saves to a SQLite database (`books.db`).
2. CSV: converts the data to a CSV file.
3. Pandas queries: filter and query a CSV file.
4. Matplotlib: draw charts from a CSV file.

## Tech

Python 3, requests, BeautifulSoup4, pandas, matplotlib, sqlite3.

## Files

- `main.py`: menu
- `BookScraper.py`: scraping, SQLite and CSV export
- `pan.py`: pandas queries
- `matplot.py`: charts
- `books.csv`, `books.db`: sample output from an earlier run (40 books)

## Run

    pip install requests beautifulsoup4 pandas matplotlib
    python main.py

## Limits

- Practice site only. No tests.
- Requests have no timeout or error handling, so a network problem can crash the script.
- The column name `Raiting` is misspelled in the saved data (kept as is).
- Menu input must be a number, other input crashes.