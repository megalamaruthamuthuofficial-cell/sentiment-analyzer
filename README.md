# 🛍️ Product Sentiment Analyzer

A web-based **Product Sentiment Analyzer** that collects product reviews from e-commerce platforms and analyzes customer sentiment.

The project uses **Selenium** for web scraping, **Flask** for the backend API, and **React.js** for the frontend.

---

## 📌 Project Overview

Product Sentiment Analyzer helps users understand customer opinions about a product by analyzing its reviews.

The application:

- 🔗 Accepts a product URL
- 🛒 Supports e-commerce product pages
- 🕷️ Scrapes customer reviews using Selenium
- 🧹 Cleans review text
- 🤖 Performs sentiment analysis
- 📊 Generates sentiment insights
- 📈 Displays results through charts
- 📋 Displays analyzed reviews in a table

---

## ✨ Features

### 🔗 Product URL Analysis
Users can enter a product URL and analyze its reviews.

### 🕷️ Web Scraping
Selenium is used to collect customer reviews from supported e-commerce websites.

### 🧹 Text Cleaning
Review text is cleaned by:

- Converting text to lowercase
- Removing HTML tags
- Removing special characters
- Removing extra spaces

### 🤖 Sentiment Analysis

Reviews are classified into:

- 🟢 Positive
- 🔴 Negative
- 🟡 Neutral

The system also calculates:

- Polarity
- Subjectivity

### 📊 Sentiment Insights

The application provides:

- Total reviews
- Positive reviews
- Negative reviews
- Neutral reviews
- Sentiment percentages
- Overall sentiment

### 📈 Dashboard

The frontend contains:

- Product information
- Summary cards
- Sentiment chart
- Rating chart
- Trend chart
- Word frequency
- Review table

---

## 🛠️ Technologies Used

### Frontend

- React.js
- JavaScript
- Axios
- Chart.js
- HTML
- CSS

### Backend

- Python
- Flask
- Flask-CORS

### Web Scraping

- Selenium
- WebDriver Manager

### NLP

- TextBlob

---

## 📁 Project Structure

```text
analyzer/
│
├── backend/
│   │
│   ├── app.py
│   ├── config.py
│   │
│   ├── routes/
│   │   ├── __init__.py
│   │   ├── product_routes.py
│   │   ├── analytics_routes.py
│   │   └── review_routes.py
│   │
│   ├── services/
│   │   ├── amazon_scraper.py
│   │   ├── flipkart_scraper.py
│   │   ├── sentiment_service.py
│   │   ├── text_cleaner.py
│   │   └── insight_service.py
│   │
│   └── utils/
│       ├── __init__.py
│       └── validators.py
│
├── frontend/
│   │
│   ├── package.json
│   ├── package-lock.json
│   │
│   └── src/
│       │
│       ├── components/
│       │   ├── navbar.js
│       │   ├── productURLinput.js
│       │   ├── productinfo.js
│       │   ├── summarycards.js
│       │   ├── sentimentchart.js
│       │   ├── ratingchart.js
│       │   ├── trendchart.js
│       │   ├── wordfrequency.js
│       │   └── reviewtable.js
│       │
│       ├── pages/
│       │   └── home.js
│       │
│       └── services/
│           └── api.js
│
└── README.md
