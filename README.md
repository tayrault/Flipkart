# 🛒 Flipkart Retail Data Analysis project

A full-cycle data analysis project built on a synthetic Flipkart retail dataset — from raw data exploration to an interactive Power BI dashboard with multi-currency support.

---

## 📌 Project Links

| Resource | Link |
|---|---|
| 📦 Dataset (Kaggle) | [Flipkart Retail Product Dataset](https://www.kaggle.com/datasets/rohiteng/flipkart-retail-product-dataset) |
| 📓 Google Colab Notebook | [Exploratory Analysis](https://colab.research.google.com/drive/1wckeagrlSKU19C6ZyyYRCwDTAhd9e8rF?usp=sharing) |
| 🗄️ Google BigQuery | [flipkart-project-487707](https://console.cloud.google.com/bigquery?ws=!1m4!1m3!3m2!1sflipkart-project-487707!2sflipkart_project) |
| 📊 Power BI Report | [Flipkart Dashboard](https://1drv.ms/u/c/ebf102a84dc0c44f/IQDw9u_QW-YIR7dcYUp8hILoAejT1Zd7sg0_Ie4pI3USRXk?e=AbxiKB) |
| 🎤 Pitch Presentation | [Google Slides](https://docs.google.com/presentation/d/1uBAihUSJsx2MBXPPH4YxPADRe5ByFZhu68LgQaqMhLo/edit?usp=sharing) |

---

## 🗂️ Dataset Overview

The dataset simulates a real-world e-commerce retail environment on Flipkart India, covering **80,000 products** sold between **2018 and 2023**.

### Key figures

| Metric | Value |
|---|---|
| Total products | 80,000 |
| Total revenue | ₹4,762 bn |
| Categories | 8 |
| Brands | 15 |
| Sellers | 8 |
| Total stock available | ~40M units |

### Categories
Appliances · Beauty · Electronics · Fashion · Home & Kitchen · Mobiles · Sports · Toys

### Brands
Adidas · Apple · Boat · Dell · HP · LG · Nike · Philips · Prestige · Puma · Redmi · Reebok · Samsung · Sony · Whirlpool

### Sellers
BestBuy · MegaStore · QuickShop · RetailHub · SmartDeals · SuperMart · UrbanRetails · ValueKart

---

## 🔬 Exploratory Data Analysis

**Tool:** Google Colab (Python)

The notebook covers:

- **Data loading & cleaning** — handling missing values, type casting, outlier detection
- **Univariate analysis** — distributions of price, rating, discount, units sold
- **Category & brand analysis** — revenue split, product count, pricing patterns
- **Seller analysis** — revenue per SKU, stock levels, geographic distribution
- **Time series** — revenue trends from 2018 to 2023 by category and brand
- **Correlation analysis** — relationships between rating, discount, and sales volume

### Key findings from EDA

- All 8 categories are **balanced in revenue share (~12.5% each)** and product count, indicating stable pricing across categories.
- Revenue per SKU consistently ranges between **₹58bn and ₹60bn** across all sellers, confirming a healthy competitive balance.
- **Value ratio is stable across brands** (~1.26%–1.28%), meaning no brand significantly over- or under-prices relative to its sales volume.
- Top 10 brands all maintain stock availability, with no major stockout risk detected.

---

## 📊 Power BI Report

**Tool:** Power BI Desktop

The report contains multiple pages analysing the Flipkart dataset across four dimensions:
| **Revenue trends** | Revenue by Year/Month split by category and brand (area chart) |
| **Category & brand split** | Revenue and product count donut charts + summary table |
| **Brand performance** | Units sold vs stock available · Value ratio vs average rating |
| **Seller performance** | nb SKUs, Revenue, Revenue per SKU, Stock available per seller |

### Currency Converter

The report includes a **live currency slicer** at the top of the page, allowing users to switch all monetary values between:

- 🇮🇳 **INR** (Indian Rupee) — base currency
- 🇪🇺 **EUR** (Euro) — 1 INR ≈ 0.011 EUR
- 🇺🇸 **USD** (US Dollar) — 1 INR ≈ 0.012 USD
---

## 🛠️ Tech Stack

| Tool | Usage |
|---|---|
| Python (Google Colab) | Exploratory Data Analysis |
| Google BigQuery | Data storage & SQL querying |
| Power BI Desktop | Interactive dashboard & DAX measures |
| GitHub | Version control & documentation |

---

## 🚀 How to Use

1. **Explore the data** — open the [Colab notebook](https://colab.research.google.com/drive/1wckeagrlSKU19C6ZyyYRCwDTAhd9e8rF?usp=sharing) to reproduce the EDA
2. **Query the data** — connect to the [BigQuery project](https://console.cloud.google.com/bigquery?ws=!1m4!1m3!3m2!1sflipkart-project-487707!2sflipkart_project)
3. **View the dashboard** — open the [Power BI report](https://1drv.ms/u/c/ebf102a84dc0c44f/IQDw9u_QW-YIR7dcYUp8hILoAejT1Zd7sg0_Ie4pI3USRXk?e=AbxiKB) and use the **currency slicer** to switch between INR, EUR, and USD
