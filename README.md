# Python_EDA_Project
### Online_Retail_Analysis

---

## Project Overview:
- This project performs Exploratary Data Analysis Aka **(EDA)** on **UK** based Online Retail data to uncover trends, patterns, customer segmentation, and also customer churn analysis. Using libraries like **Pandas, Matplotlib** for cleaning, Visualization, and analysis.
- In this project I used FireDucks library and analyzed **32 mil** records to save the tons of time.

## Objective
1. Analyze large dataset products, Description, and StockCode from different Country.
2. Understanding the customer purchase behaviour and keep them by offering active promotions.
3. Identify the trends across the different country.
4. Detect churn customers and Analyze RFM.

---

## Dataset
- **Invoiceno:** Unique invoiceno 
- **StockCode:** It's an item code or a product code
- **Description:** The Name of the item or product
- **Quantity:** The Total Quantity of the item bought
- **InvoiceDate:** Date of purchase of the item/product
- **UnitPrice:** Unit Price for each item/product
- **CustomerID:** ID for each customer who bought an item from the store
- **Country:** Where the item/product was purchased

## Workflow

### 1. Data Cleaning
- **Handle missing values:** `Description`, `CustomerID` columns had null values
- **Fix Description using mode:** picked specific `StockCode` and fixed their Description based on frequent using `Description.mode()`
- **Add Index:** The way this function works will short the records which has the highest counts will appear at the top.
- **Using Groupby:** Performed a group by on this particular dataframe using `StockCode`. It shows the most frequent valid description along with the counts.

  ### 2. Feature Engineering
  - **Add TotalSales:** Created a new column in the table as `TotalSales`, calculated as `Quantity * UnitPrice`
  



















