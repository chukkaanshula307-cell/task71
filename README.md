# PriceTracker

## Overview

PriceTracker is a lightweight, single‑file web application that allows users to:

* Track product prices
* Monitor price changes over time
* Set target price alerts
* Compare prices across stores (mock comparisons)
* View auto‑generated charts for price history
* Store and manage tracked products using localStorage


---

## Features

### Add Products

Users can enter a product name, optional store URL, current price, target price, category, and store.

### Track Price History

Each product maintains a history of prices. When prices are simulated, new entries are added automatically.

### Price Alerts

Notifications appear when:

* A product’s current price reaches or drops below the target price.

### Filtering

Users can filter tracked products by:

* Category
* Store

### Charts

* **Line chart:** Displays historical price trends for the selected product.
* **Bar chart:** Compares store prices using generated mock values.

### Light/Dark Theme

Users can toggle between light and dark mode.

### Data Persistence

All tracked products are saved in **localStorage**, so data stays even after refreshing the page.

---

## How It Works

### 1. Adding a Product

When a user adds a product:

* It is assigned a unique ID.
* The initial price is saved to the history array.
* The product appears in the tracked list.

### 2. Simulated Price Updates

Clicking **Simulate price fetch**:

* Randomly adjusts product price.
* Adds a new entry to price history.
* Triggers alerts if target price is met.

### 3. Viewing Price Charts

Selecting a product updates:

* Line chart → product price history
* Bar chart → mock comparisons across stores

---

## File Structure

This project is built in a **single HTML file**, containing:

* HTML layout
* CSS styling
* JavaScript application logic
* Embedded Chart.js integration

No external files are required besides the Chart.js CDN.

---

## How to Use

1. Open the HTML file in any modern browser.
2. Add products using the input fields.
3. Use **Simulate price fetch** to generate random price updates.
4. Click **View** on any product to load its historical chart.
5. Apply category/store filters as needed.
6. Switch themes using **Dark Mode** toggle.

---

## Requirements

* A modern web browser (Chrome, Edge, Firefox, Safari)
* Internet connection (only for loading Chart.js CDN)

---

## Notes

* Price values in comparison charts are mock values.
* The application does not fetch real‑time prices unless extended with APIs.
* Designed strictly for demonstration and academic purposes.

---

## Future Enhancements

* Real API integration for live price tracking
* User authentication and cloud sync
* Exportable reports and charts
* Enhanced UI/UX with animations and improved layouts

---

