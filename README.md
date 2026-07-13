# Diwali Retail Sales Exploratory Data Analysis (EDA)

This repository contains a comprehensive data analytics project focused on evaluating customer purchasing behaviors and retail trends during the Diwali festive season. Using Python and core data science libraries, this analysis transforms raw transactional data into actionable business intelligence.

## Project Objective

The primary objective of this project is to perform a detailed Exploratory Data Analysis (EDA) on Diwali festival sales data to uncover hidden consumer purchasing patterns and operational trends. 

By analyzing transactional retail data, this project aims to:
* **Identify High-Value Customer Segments:** Determine which demographics (gender, age group, occupation, marital status) contribute most significantly to overall revenue.
* **Optimize Inventory & Supply Chain:** Pinpoint the top-selling product categories and specific items to help retail managers optimize stock levels during peak festive seasons.
* **Enhance Targeted Marketing Strategies:** Map geographical sales distribution across states and zones to provide data-backed recommendations for localized, high-ROI marketing campaigns.
* **Improve Business Decision-Making:** Transform raw transactional data into actionable insights that help retail stakeholders predict future holiday sales behaviors and optimize pricing strategies.


## Datasets Used

- <a href="https://github.com/mohdnaved04/Diwali-Sales-Analysis-/blob/main/Diwali%20Sales%20Data%20(1).csv">Diwali Dataset</a>
- <a href="https://github.com/mohdnaved04/Diwali-Sales-Analysis-/blob/main/Diwali_Sales_Analysis.ipynb">Python Analysis</a>

> **Data Note:** The raw dataset initially contained completely blank columns (`Status` and `unnamed1`) and minor null values in the `Amount` column, both of which were systematically handled during the data preprocessing phase to protect statistical integrity.

## Questions & KPIs Analyzed

### **Key Performance Indicators (KPIs)**
1. **Total Sales Revenue:** Total monetary value generated across all transactions.
2. **Total Orders:** Cumulative count of items purchased.
3. **Average Order Value (AOV):** The average amount spent per transaction.
4. **Demographic Sales Distribution:** Revenue breakdown by age, gender, and occupation.

### **Core Business Questions Answered**
* **Gender Dynamics:** Who spends more money and places more orders between men and women?
* **Age Distribution:** Which age bracket represents the core purchasing power of the consumer base?
* **Marital Impact:** Does marital status influence overall spending patterns and product preferences?
* **Geographic Powerhouses:** Which states and zones generate the maximum revenue and order volume?
* **Occupational Insights:** Which professional sectors do the top-spending customers belong to?
* **Product Dominance:** Which product categories are the most popular, and which ones generate the highest total revenue?

## Data Analysis & Development Process

The project followed a structured data science workflow from raw data ingestion to generating final business insights:

[Data Cleaning] ➔ [Exploratory Data Analysis] ➔ [Data Visualization] ➔ [Insights Generation]

### 1. Data Cleaning & Preprocessing
Before diving into analysis, the dataset was systematically cleaned to ensure absolute data integrity and optimize performance:
*   **Handling Encodings:** Resolved file-loading errors (`UnicodeDecodeError`) by importing the data using alternative encodings (`latin1` / `cp1252`)[cite: 1].
*   **Dropping Redundant Columns:** Permanently removed completely blank columns (`Status` and `unnamed1`) to streamline the dataframe and optimize memory usage[cite: 1].
*   **Handling Missing Values:** Identified and dropped rows containing null values within the `Amount` column to protect numerical accuracy in downstream calculations[cite: 1].
*   **Data Type Conversion:** Cast the `Amount` column from a `float` to an `int` for cleaner data modeling, faster processing, and precise currency aggregation[cite: 1].

### 2. Exploratory Data Analysis (EDA)
Leveraged core scientific computing libraries to uncover high-level trends:
*   **Descriptive Statistics:** Applied `Pandas` and `NumPy` methods to extract baseline metrics (mean, median, distributions, and variance)[cite: 1].
*   **Categorical Aggregation:** Grouped, aggregated, and sorted data across multiple dimensions (e.g., grouping `Amount` by `Age Group` and sorting by total spend) to immediately isolate top revenue-generating variables[cite: 1].

### 3. Data Visualization
Translated numbers into compelling visual narratives using `Matplotlib` and `Seaborn`[cite: 1]:
*   **Custom Chart Design:** Engineered dynamic bar charts, count plots, and stacked visualizations to map complex customer demographic breakdowns, regional performance, and product hierarchies[cite: 1].
*   **Enhanced Scannability:** Programmed explicit data labels onto chart bars, making precise metric figures instantly visible to stakeholders without sacrificing visual elegance.

### 4. Insights Generation & Documentation
*   **Executive Synthesis:** Extracted clear visual patterns and translated data relationships into concrete, strategic business recommendations.
*   **Reproducibility:** Fully annotated the Jupyter Notebook with rich markdown cells, code documentation, and clean separation of concerns to ensure the analysis pipeline can be reliably reproduced or scaled[cite: 1].
