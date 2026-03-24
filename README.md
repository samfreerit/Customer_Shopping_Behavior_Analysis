# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using Python for data cleaning, preprocessing, exploratory data analysis (EDA), and database integration.

The goal is to understand customer purchase patterns, category preferences, age-based behavior, review ratings, discounts, and purchase frequency to generate business insights useful for retail decision-making.

---

## Project Objectives

* Clean and preprocess customer shopping dataset
* Handle missing values in review ratings
* Standardize column names for analysis
* Create customer age groups
* Convert purchase frequency into numerical values
* Identify relationships between discounts and promo code usage
* Store processed data into SQL databases

---

## Technologies Used

* Python
* Pandas
* NumPy
* SQLAlchemy
* PostgreSQL
* MySQL
* Jupyter Notebook

---

## Dataset Features

The dataset includes:

* Age
* Category
* Purchase Amount
* Review Rating
* Discount Applied
* Promo Code Used
* Frequency of Purchases

---

## Data Preprocessing Steps

### 1. Missing Value Handling

Missing values in **Review Rating** are filled using category-wise median values.

### 2. Column Standardization

Column names are converted into lowercase and spaces are replaced with underscores.

### 3. Feature Engineering

Created:

* `age_group`
* `purchase_frequency_days`

### 4. Redundant Column Removal

Removed duplicate business information from:

* `promo_code_used`

---

## Age Group Classification

Customers are divided into:

* Young Adult
* Adult
* Middle-aged
* Senior

---

## Purchase Frequency Mapping

Purchase frequency converted into numeric days:

* Weekly → 7
* Fortnightly → 14
* Monthly → 30
* Quarterly → 90
* Annually → 365

---

## Database Integration

Processed data is exported into SQL databases:

### MySQL

Used SQLAlchemy with pymysql for MySQL export.

---

## Project Structure

```bash
Customer_Shopping_Behavior_Analysis/
│── Customer_Shopping_Behavior_Analysis.ipynb
│── README.md
│── Customer Behaviour VT.mp4
│── dataset.csv
```

---

## Sample Insights

* Customer age impacts shopping frequency
* Discounts strongly influence purchase behavior
* Product categories show different review rating trends

---







