# DataSpark: Illuminating Insights for Global Electronics

## Project Overview

**DataSpark** is a comprehensive data analytics project focused on Retail Analytics in the Electronics Industry. This project involves data cleaning, preprocessing, exploratory data analysis (EDA), and visualization using Python, SQL, and Power BI/Tableau. The primary goal is to generate actionable insights from a global dataset of electronics sales.

## Features

- **Data Cleaning & Preprocessing**: Removing missing values, formatting data, and standardizing column names.
- **Data Storage**: Storing cleaned data into a MySQL database.
- **Data Analysis**: Running SQL queries to generate key insights such as customer demographics, sales performance, and product popularity.
- **Data Visualization**: Creating dashboards in Power BI to visualize and report the analysis.

## Data Sources

- **Sales.csv**: Contains sales transactions with details such as order number, order date, customer, store, product, quantity, and currency code.
- **Products.csv**: Contains product details including product name, brand, color, unit cost, unit price, subcategory, and category.
- **Stores.csv**: Contains store details including store key, country, state, square meters, and open date.
- **Exchange_Rates.csv**: Contains exchange rates with details such as date, currency, and exchange rate.
- **Customers.csv**: Contains customer details including customer key, gender, name, city, state code, state, zip code, country, continent, and birthday.

## Data Cleaning & Preprocessing

### Missing Values Handling

- Dropped the `Delivery Date` column from `sales_df`.
- Filled missing values in the `Square Meters` column of `stores_df` with 0.
- Filled missing values in the `State Code` column of `customers_df` with 'NAP'.

### Data Formatting

- Converted currency columns to float after removing '$' and ',' symbols.
- Converted date columns to `datetime` format.
- Standardized zip codes to 5 digits.
- Applied consistent title casing for city and country names.
- Mapped state names to their corresponding state codes where necessary.
- Removed trailing product specifications from `Product Name`.

### Storing Data in MySQL

1. Database Configuration
2. Create Tables
3. Load Data into MySQL

## Data Analysis Queries

1. Number of Customers by Gender
2. Number of Customers from Each Continent
3. Customers from Each State
4. Year-wise Total Revenue
5. Top 20 Selling Products
6. Ranking Brands by Quantities Sold
7. Top Sold Categories
8. Subcategories and Quantities Sold
9. Sales by Stores (Country-wise)
10. Sales by Stores (State-wise)
   
## Data Visualization

The insights from the above queries were visualized in Power BI, creating interactive dashboards to help stakeholders make data-driven decisions. 

Power BI Dash Board ([Power BI DashBoard.png](https://github.com/JayanthiML/DataSpark-Illuminating-Insights-with-Power-BI/blob/main/Power%20BI%20DashBoard.png))

## Conclusion

**DataSpark** demonstrates the power of data cleaning, preprocessing, and visualization in uncovering valuable insights from large datasets. By using Python for data manipulation and MySQL for data storage, along with Power BI for visualization, we can provide a robust analytical framework for the global electronics industry.

This README file provides a clear overview of your project, covering all the major aspects from data handling to analysis and visualization.
