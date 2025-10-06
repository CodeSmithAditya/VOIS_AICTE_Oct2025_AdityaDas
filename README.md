# Exploratory Data Analysis of NYC Airbnb Listings

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7%2B-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12%2B-purple)

## 1. Project Overview

This project provides a thorough exploratory data analysis (EDA) of the New York City Airbnb open dataset. The primary goal is to perform a detailed data cleaning process and then derive actionable insights by analyzing and visualizing trends related to listings, pricing, host activity, and guest reviews.

This analysis was completed as a project for the **VOIS for Tech Program**, an internship initiative by VOIS and the Vodafone Idea Foundation through AICTE.

---

## 2. Project Workflow

The analysis was conducted in a structured manner, following standard data science practices:

### Data Cleaning and Preprocessing
The raw dataset underwent a rigorous cleaning process to ensure data quality and consistency. Key steps included:
* **Handling Duplicates:** Removed all duplicate records.
* **Managing Missing Data:** Dropped columns with insufficient data (`house_rules`, `license`) and removed rows with remaining null values.
* **Correcting Data Types:** Converted columns to their appropriate types (e.g., `price` to float, `last review` to datetime, `Construction year` to integer).
* **Data Formatting:** Cleaned numeric columns (`price`, `service fee`) by removing symbols like '$' and commas.
* **Fixing Categorical Errors:** Corrected misspellings in categorical data (e.g., 'brookln' to 'Brooklyn').
* **Outlier Removal:** Filtered out outlier data points to ensure statistical accuracy.

### Exploratory Data Analysis (EDA)
Following the cleaning phase, an in-depth EDA was performed to answer key business questions through statistical summaries and visualizations.

---

## 3. Key Questions and Findings

This analysis sought to answer the following questions:

1.  **What are the different property types available?**
    * **Finding:** The dataset is dominated by **'Entire home/apt'** and **'Private room'**, with 'Shared room' being a very small fraction of the listings.

2.  **Which neighborhood group has the highest number of listings?**
    * **Finding:** **Manhattan** and **Brooklyn** are the clear leaders, containing the vast majority of all Airbnb listings in NYC.

3.  **Which neighborhood group has the highest average prices?**
    * **Finding:** **Manhattan** has the highest average listing price, making it the most expensive borough for Airbnb stays.

4.  **What is the relationship between a property's construction year and its price?**
    * **Finding:** The analysis revealed **no clear or consistent correlation** between the construction year and the average price of a listing.

5.  **Who are the top 10 hosts by listing count?**
    * **Finding:** A small number of hosts (likely property management companies) manage a disproportionately large number of listings, with the top host controlling hundreds of properties.

6.  **Are hosts with verified identities more likely to receive positive reviews?**
    * **Finding:** There is a **negligible difference** in average review scores between verified and unverified hosts, suggesting guests do not factor this into their ratings significantly.

7.  **Is there a correlation between the price and the service fee?**
    * **Finding:** A **near-perfect positive correlation (r ≈ 0.99)** exists. This strongly indicates that the service fee is a direct percentage of the listing price.

8.  **How does the average review rate (stars) vary by location and room type?**
    * **Finding:** Most properties cluster around an average review rating of **3 out of 5 stars**, with only minor variations across different neighborhood groups and room types.

9.  **Are hosts with more listings more likely to have higher availability?**
    * **Finding:** There is only a **very weak positive correlation**, meaning the number of properties a host manages is not a reliable predictor of their availability.

---

## 4. Technologies Used

* **Python:** The core programming language for the analysis.
* **Pandas:** Used for data manipulation, cleaning, and aggregation.
* **Matplotlib & Seaborn:** Used for generating static and statistical visualizations.
* **Jupyter Notebook (Google Colab):** The interactive environment for writing and executing the code.

---

## 5. How to Run This Project

To reproduce this analysis, follow these steps:
1.  Clone or download this repository.
2.  Ensure you have a Python environment with the libraries listed above installed.
3.  Place the dataset (`1730285881-Airbnb_Open_Data.csv`) in the same directory as the Jupyter Notebook (`VOIS_Airbnb_Project_AdityaDas.ipynb`).
4.  Open and run the notebook cells in sequential order.
