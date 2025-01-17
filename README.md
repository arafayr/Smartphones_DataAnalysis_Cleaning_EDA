# Data Cleaning and Exploratory Data Analysis On Smartphones

This project focuses on analyzing smartphone data to uncover patterns and trends. It involves cleaning the dataset and performing exploratory data analysis (EDA) to extract meaningful insights.

## Files in the Repository

1. **Cleaning_of_smartphone_data.ipynb**:
   * This notebook handles the initial cleaning of the smartphone dataset, addressing data quality and tidiness issues.
   - Key steps include:
     - Detecting and correcting quality issues such as:
       - Removing special characters from the price column.
       - Handling inconsistent brand names .
       - Correcting missing or incorrect values in columns like `ratings`, `processor`, and `memory`.
       - Identifying outliers like feature phones or special addition phones.
     - Splitting columns for better data structure:
       - Example: Splitting `sim` into `has_5G`, `has_NFC`, and `has_IR_Blaster`.
     - Resolving shifted data (e.g., misplaced `sim` data in the `processor` column).
     - Imputing missing values for columns like `ratings`.

2. **EDA_smartphone.ipynb**:
   - This notebook explores the cleaned dataset to understand the relationships between various features.
   - Key analyses include:
     - **Univariate Analysis**:
       - Examining individual columns such as `brand`, `price`, and `ratings` for distribution, skewness, and outliers.
       - Highlighting key observations like:
         - Price column is highly skewed with many outliers.
         - Most phones have features like 5G and fast charging.
     - **Bivariate Analysis**:
       - Analyzing relationships between features, e.g.:
         - `Brand` vs `Price`: Less-known brands like iQOO have higher average prices.
         - `Processor Name` vs `Price`: Apple processors are associated with higher price ranges.
         - `Processor Speed` vs `Price`: High-range phones have processor speeds above 2.8 GHz.
         - `5G` vs `Price`: Phones with 5G tend to be in the mid-range to high-range price category.
       - Observing how specific features affect price, such as NFC and IR blasters.

## Key Insights

- **Price Trends**:
  - Low-range phones end at 25k, mid-range phones at 60k, and high-end phones reach 2 lacs.
  - Phones with features like NFC and faster processors have higher average prices.
  - Qualcomm processors are the most common but are associated with mid-range prices.
  - High-end phones are often equipped with Apple processors, reflecting their premium pricing strategy.
  - Phones with fast charging are dominant in the dataset, showing a market trend toward quick charge capabilities.
  - IR blasters are mainly provided by Chinese brands, such as Xiaomi, at competitive prices.
  - Low-range phones typically have speeds of 1.2–1.8 GHz.
  - Mid-range phones operate at 2.0–2.4 GHz.
  - High-end phones exceed 2.8 GHz, reflecting their superior performance capabilities.
  - Android dominates the market, but iOS devices significantly impact the price range, with higher price points linked to Apple devices.


- **Missing Data**:
  - Missing values in columns like `ratings`, `refresh rate`, and `processor brand` were handled using methods like KNN imputation.

## Future Work

- Performing multivariate analysis
- Model building


