# Flipkart Products - Data Cleaning & EDA

Data cleaning and exploratory data analysis on the Flipkart Products dataset — handling missing values, price formatting, and category inconsistencies using Python & Pandas.

## 📊 Dataset

- **Source:** [Flipkart Products Dataset (Kaggle)](https://www.kaggle.com/datasets/muhammadumer7804/flipkart-dataset)
- **Size:** 20,000 product listings
- **Columns:** 15 (product name, price, category, brand, description, ratings, etc.)

## 🎯 Project Objective

Real-world e-commerce data is often messy — missing values, inconsistent formatting, and unstructured text fields. This project demonstrates a complete data cleaning and EDA workflow to transform raw Flipkart product data into a clean, analysis-ready dataset, followed by visual exploration of pricing and category trends.

## 🧹 Data Cleaning Steps

| Step | Action | Result |
|------|--------|--------|
| Missing Prices | Removed rows with missing `retail_price` / `discounted_price` | 78 rows removed |
| Missing Brand | Filled missing values with "Unknown" | 5,864 values filled |
| Missing Description/Image/Specs | Removed rows with missing values | 17 rows removed |
| Duplicates | Checked for duplicate `uniq_id` | 0 duplicates found |
| Price Logic | Verified discounted price never exceeds retail price | 0 errors found |
| Category Extraction | Extracted main category from nested category tree | 263 → 33 clean categories |

**Final dataset:** 19,905 clean rows, 0 missing values.

## 📈 Exploratory Data Analysis

- **Category Distribution** — Clothing (6,167) and Jewellery (3,521) dominate the catalog
- **Price Distribution** — Right-skewed; most products priced under ₹2,500
- **Retail vs Discounted Price** — Strong proportional relationship, with wider discount variation at higher price points
- **Discount Percentage** — Average discount of 40.5% (median 45%); notable spikes at 0% and 50%
- **Category-wise Pricing** — Furniture has the highest average price (₹23,263); Sunglasses and Wearable Smart Devices have the highest average discounts (~58%)
- **Brand Analysis** — Top real brands include Allure Auto, Voylla, and Karatcraft

## 🛠️ Tools & Libraries

- **Python**
- **Pandas** — data cleaning and manipulation
- **Matplotlib / Seaborn** — data visualization

## 📁 Repository Structure

```
flipkart-products-data-cleaning-eda/
├── flipkart-products-data-cleaning-eda.ipynb   # Main notebook
├── README.md
└── LICENSE
```

## 🚀 How to Run

1. Clone this repository
2. Download the dataset from Kaggle and place it in the working directory
3. Open `flipkart-products-data-cleaning-eda.ipynb` in Jupyter Notebook, Google Colab, or Kaggle
4. Run all cells sequentially

## 📌 Key Takeaways

This project highlights common real-world data quality issues — missing values, inconsistent category formatting, and mixed-format text fields — and demonstrates practical, step-by-step techniques to clean and analyze them using Pandas.

## 👤 Author

Muhammad Umer as Aiwriter404.

---

*This project is part of my ongoing learning in Python and Data Analytics.*
