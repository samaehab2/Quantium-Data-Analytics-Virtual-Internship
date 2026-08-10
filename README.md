# Retail Data Analytics & Customer Segmentation
An end-to-end data analytics project focused on transaction data cleaning, exploratory data analysis (EDA), customer segmentation, and purchasing behavior insights for a retail supermarket brand.

 # Project Overview
This project processes and analyzes large-scale customer transaction records to identify purchasing trends, customer lifestage behaviors, and high-value customer segments. The insights generated help optimize inventory management, target marketing strategies, and drive sales growth.

# Key Objectives
Clean raw transaction and customer behavior datasets.
Handle Excel date conversions, missing values, and outliers using statistical methods (IQR).
Perform feature engineering (extract pack sizes, filter non-target categories like Salsa).
Identify key sales trends, seasonal patterns (e.g., pre-Christmas demand spikes), and store closures.
Segment customers by Lifestage and Premium Type to pinpoint core revenue drivers.

# Tech Stack & Tools
Language: Python 3.x
Data Manipulation: pandas, numpy
Data Visualization: matplotlib, seaborn
Pattern Matching: re (Regular Expressions)
Environment: Jupyter Notebook / VS Code

# Workflow & Data Pipeline

1. Data Cleaning & Preprocessing:
>Outlier Removal: Filtered extreme price/quantity values using the Interquartile Range (IQR) methodز
>Date Normalization: Converted Excel integer dates to standard datetime formats (origin 1899-12-30).
>Category Filtering: Removed non-chip products (e.g., Salsa dips) to isolate the target snack category.

2. Feature Extraction:
>Extracted numerical product pack sizes (in grams) using Regular Expressions (re).
>Categorized transaction types and customer types for group-level aggregation.

3. Time-Series & Trend Analysis:
>Aggregated daily total sales to detect seasonal peaks.
>Identified store closure on Christmas Day (Dec 25) by cross-referencing a full 365-day calendar index.
>Analyzed pre-Christmas demand surges to recommend stock preparation timelines.

4. Customer Segmentation:
>Merged cleaned transaction data with customer demographic data via LYLTY_CARD_NBR.
>Evaluated sales contributions across LIFESTAGE (e.g., Young Singles/Couples, Retirees, Mainstream) and PREMIUM_CUSTOMER tiers (Budget, Mainstream, Premium).

# Key Insights & Business Recommendations:
>Pre-Christmas Sales Peak: High sales volume concentrated in the 18–24 December period; inventory levels should be ramped up 2 weeks prior.
>Target Audience: Mainstream Young Singles/Couples and Budget Retirees contribute significantly to total pack volume and overall revenue.
>Pack Size Preference: Larger pack sizes yield higher overall revenue per transaction, presenting an opportunity for targeted promotional bundle offers.















