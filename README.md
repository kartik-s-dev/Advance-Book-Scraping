# 📚 Advance Book Scraping & Analysis Tool

A powerful, automated Python tool designed to scrape book data from e-commerce/web sources, process and clean the data, store it in structured databases (SQLite & CSV), and provide insightful visual analytics using Pandas and Matplotlib.

---

## ✨ Features

- **Automated Web Scraping:** Scrapes book titles, prices, ratings, and availability automatically.
- **Data Persistence:** Saves extracted data directly into `CSV` files and `SQLite` databases (`books.db`).
- **Data Analysis & Filtering:** Built-in Pandas queries to filter books by price, rating, and custom conditions.
- **Data Visualization:** Generates visual graphs using Matplotlib for price trends and category distribution.
- **Interactive CLI:** Easy-to-use command-line interface to run scraper, save files, and execute queries.

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python 3.x
- **Scraping:** BeautifulSoup4, Requests
- **Data Handling:** Pandas, SQLite3
- **Visualization:** Matplotlib

---

## 📁 Project Structure

```text
Advance-Book-Scraping/
│
├── main.py                   # Main CLI Entry Point
├── BookScraper.py            # Web scraping logic
├── pan.py                    # Pandas data processing & query execution
├── matplot.py                # Data visualization & graphing module
├── book.csv / books.csv      # Extracted datasets
└── books.db                  # SQLite database file
