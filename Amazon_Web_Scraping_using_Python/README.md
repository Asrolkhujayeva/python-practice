# 🛒 Amazon Price Tracker (Web Scraping Project)

This is a simple Python script that **monitors the price** of a specific Amazon product and **automatically appends the latest data to a CSV file** every 24 hours.

---

## 📌 Project Overview

The script sends a request to the product page on Amazon, extracts the **product title** and **current price**, and records the information along with the current date in a `.csv` file. This allows you to **track price changes over time**.

---

## 💻 Tools & Libraries Used

- `requests` – for sending HTTP requests to the Amazon page  
- `BeautifulSoup` (bs4) – for parsing and extracting HTML content  
- `csv` – for saving data  
- `datetime` – for tracking when data was collected  

---

## 🔁 Functionality

- Automatically runs once every 24 hours (using an external scheduler like Task Scheduler or cron)
- Extracts:
  - Product title
  - Current price (`$XX.XX`)
  - Date of last check
- Appends the result to a CSV file:
