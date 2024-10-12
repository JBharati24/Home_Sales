# Home Sales Analysis Assignment

## Overview

This repository contains the code and analysis for the Home Sales Assignment conducted using PySpark in Google Colab. The primary objective of this assignment is to analyze home sales data to extract insights about home prices based on various attributes like the number of bedrooms, bathrooms, view ratings, and year built.

## Dataset

The dataset used in this analysis is sourced from an AWS S3 bucket and includes information about home sales, including:

- ID
- Date of Sale
- Date Built
- Price
- Bedrooms
- Bathrooms
- Square Feet
- View Rating

The dataset is stored in a CSV file named `home_sales_revised.csv`.

## Key Steps

1. **Environment Setup**
   - Installed Java and Spark.
   - Set up environment variables for Spark.

2. **Data Loading**
   - Loaded the dataset from the AWS S3 bucket into a Spark DataFrame.
   - Created a temporary view of the DataFrame for SQL queries.

3. **Data Analysis**
   - Performed various SQL queries to analyze the dataset, including:
     - Average price of four-bedroom houses sold per year.
     - Average price of homes based on the number of bedrooms and bathrooms.
     - Average price of homes with specific criteria (e.g., number of floors, square footage).
     - Average price of homes based on view ratings.
   - Caching temporary tables to improve query performance.

4. **Data Storage**
   - Saved the processed DataFrame as a partitioned Parquet file for optimized storage and retrieval.

5. **Performance Comparison**
   - Compared runtimes of queries before and after caching, and also with the Parquet formatted data.

## Technologies Used

- Python
- PySpark
- Google Colab

## Instructions to Run

1. Open the Google Colab notebook in this repository.
2. Ensure all required libraries are available and installed.
3. Run the cells sequentially to perform the analysis.

## Conclusion

This assignment provides valuable insights into home sales data, demonstrating the power of PySpark for big data analysis. The analysis showcases how to use SQL queries to extract meaningful information from a dataset, making it a crucial skill for data analysts.
