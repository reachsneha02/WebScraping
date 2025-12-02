# Web Scraping, Extracting and Visualization of Stocks data

This project showcases my skills in **web scraping, data wrangling, and visualization** using Python.  
I work with real financial data to extract:

- Historical stock prices using the `yfinance` API  
- Quarterly revenue data by scraping HTML tables from the web  

and then combine everything into a simple **dashboard-style visualization**.

The stocks analyzed in this project are:

- Apple (AAPL)
- Amazon (AMZN)
- GameStop (GME)

---

## 1. Background and Motivation

Web scraping (also known as web harvesting or web data extraction) is a key technique in data science for turning **unstructured web content** into **structured datasets** that can be analyzed. It can be used to extract large amounts of data from websites. It is a primary method of collecting data from the internet, and can be used for real-time applications.
 
A stock (also known as equity) is a security that represents the ownership of a fraction of a corporation . This Entitles the owner of the stock to a proportion of the corporation's assets and profits equal to how much stock they own. Units of stock are called "shares." An investor can buy a stock and sell it later. If the stock price increases, the investor profits. If it decreases, the investor will incur a loss. Determining the stock price is complex; it depends on the number of outstanding shares, the size of the company's future profits, and much more. People trade stocks throughout the day. 

The stock ticker is a report of the price of a certain stock, updated continuously throughout the trading session by the various stock market exchanges. The yfinance is a Python library with a user-friendly interface for downloading historical market data from Yahoo Finance. It lets you get historical stock prices, dividends, and other financial data for stocks, exchange-traded funds (ETFs), and other securities.

The goal is to help understand how **stock prices** relate to **company fundamentals (revenue)** by:

- Extracting historical stock price data
- Scraping quarterly revenue data from financial websites
- Cleaning and transforming the data
- Visualizing both on a dashboard to identify patterns and trends

This mini-project demonstrates a realistic workflow that is common in data-driven roles.

---

## 2. What This Project Demonstrates

**Technical skills:**

- Using `yfinance` to download historical market data from Yahoo Finance
- Using `requests`, `BeautifulSoup`, and `pandas.read_html` to scrape HTML tables
- Cleaning messy web data with `pandas`:
  - Parsing dates
  - Removing currency symbols and commas
  - Handling missing/empty values
  - Resetting indices and renaming columns
- Building a reusable plotting function using **Matplotlib** to visualize:
  - Stock price over time
  - Quarterly revenue over time
- Structuring analysis in a clear, reproducible Jupyter Notebook

**Data science skills:**

- Turning unstructured web content into tabular data
- Combining multiple data sources (API + web scraping)
- Creating intuitive visualizations that connect price action with fundamentals

---
## 3. Project Structure

```text
.
├─ WebScraping_DataExtraction_Visualization.ipynb   # Main Jupyter Notebook                                  
└─ README.md                    # Project documentation

```

## 4. Notebook Contents and Workflow

### High-level notebook flow

1. **Import libraries and set up**
   - `pandas`, `matplotlib`
   - `yfinance`
   - `requests`, `BeautifulSoup` for web scraping

2. **Download stock price data**

   Use `yfinance.Ticker(...).history()` to get historical price data for:

   - Apple (**AAPL**)
   - Amazon (**AMZN**)
   - GameStop (**GME**)

3. **Scrape quarterly revenue data**

   - Use `requests.get()` to fetch HTML pages  
   - Use `BeautifulSoup` and/or `pd.read_html()` to extract revenue tables  
   - Clean the table

4. **Build a dashboard plotting function** and  **Visualize each stock**

   Define a reusable function (e.g. `make_graph`) 



## 5. Libraries and Dependencies

The notebook uses the following Python libraries:

- `pandas` – data manipulation and analysis  
- `yfinance` – download historical market data from Yahoo Finance  
- `requests` – HTTP requests to fetch web pages  
- `beautifulsoup4` – parse HTML content  
- `matplotlib` – data visualization  
- `lxml` – HTML/XML parser used by `pandas.read_html`  

You can install them with:

```bash
pip install pandas yfinance requests beautifulsoup4 matplotlib lxml
```
## 6. How to Run the Project

1. Clone or download this repository to your local machine.
2. Ensure you have **Python 3.8+** installed.
3. Install the required libraries.
4. Start Jupyter Notebook.
5. Open  WebScraping_DataExtraction_Visualization.ipynb and run the cells in order.

## 7. Summary

This project combines:

- API data access (`yfinance`)
- Web scraping (`requests`, `BeautifulSoup`, `pandas.read_html`)
- Data cleaning (`pandas`)
- Visualization (`matplotlib`)

to build a small but complete end-to-end pipeline, from raw web pages to clear visualizations.

It also demonstrates my ability to work with real-world financial data for data science and analytics roles.

