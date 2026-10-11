# BookStore Data Scraper & Analyzer

[![GitHub commit](https://img.shields.io/badge/GitHub-Commit%3A%20dfbd511-blue)](https://github.com/swarup-lature/BookStore-Data-Scraper-Analyzer)

A complete Python-based data pipeline and exploratory analysis project that extracts live book inventory data from an online bookstore, processes and cleans it using Pandas, and generates visual insights with Matplotlib.

## 🚀 Project Overview
This project automates the workflow of collecting web data, transforming raw string-based records into a structured analytical format, computing descriptive statistics, and exporting visual charts. It serves as a practical demonstration of end-to-end data manipulation from scratch.

## 🛠️ Tech Stack & Libraries
* **Python**: Core programming language used for scripting and data workflow automation.
* **BeautifulSoup & Requests**: For retrieving HTML content and parsing web DOM elements.
* **Pandas & NumPy**: For handling dataframes, missing values, regular expression string cleaning, and numerical computations.
* **Matplotlib**: For plotting and exporting exploratory visualization charts.
* **Jupyter Notebook**: Interactive development environment (`webscapping.ipynb`).

## 📊 Key Pipeline Steps
1. **Web Extraction**: Connects to the target bookstore page, locates product pods (`article` tags), and extracts attributes including book names, raw price strings, star ratings, and stock availability.
2. **Data Transformation & Cleaning**: 
   * Strips currency symbols and non-numeric characters from price strings, casting them into floating-point numbers.
   * Maps categorical text ratings (*One, Two, Three, Four, Five*) to quantitative integer values ($1$ through $5$).
3. **Exploratory Data Analysis (EDA)**: Computes dataset metrics such as total book count, average price points, mean ratings, and filters top-tier selections or most expensive entries.
4. **Data Export & Visualization**: Saves the cleaned records into a structured CSV file and generates horizontal bar charts representing top-priced books[cite: 3].

## 📁 Repository Structure
* `webscapping.ipynb`: Complete Jupyter Notebook containing the executable code for scraping, cleaning, analysis, and visualization[cite: 3].
* `scraped_books.csv`: Structured dataset containing the processed book inventory records[cite: 3].
* `README.md`: Comprehensive project documentation.

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/swarup-lature/BookStore-Data-Scraper-Analyzer.git](https://github.com/swarup-lature/BookStore-Data-Scraper-Analyzer.git)
