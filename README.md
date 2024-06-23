
![walmart 1](https://github.com/AYOUB09S/Building-a-Retail-Data-Pipeline/assets/78933570/d31be4e9-fa0c-49d3-94c5-74e1fd5d5188)

Walmart is the biggest retail store in the United States. Just like others, they have been expanding their e-commerce part of the business. By the end of 2022, e-commerce represented a roaring $80 billion in sales, which is 13% of total sales of Walmart. One of the main factors that affects their sales is public holidays, like the Super Bowl, Labour Day, Thanksgiving, and Christmas.
# Building-a-Retail-Data-Pipeline
Mastering data pipelines is essential for Data Engineers. In this project, you'll work with Walmart retail data, retrieving it from SQL and Parquet sources, transforming it using various techniques, and loading it into accessible CSV files. Key functions handle extraction, transformation, loading, and validation.

# Data Sources
## grocery_sales (PostgreSQL table)
**index: Unique ID of the row**
**Store_ID: Store number**
**Date: Week of sales**
**Weekly_Sales: Sales for the given store**
## extra_data.parquet (Parquet file)
**IsHoliday: Public holiday week (1 if yes, 0 if no)**
**Temperature: Temperature on the day of sale**
**Fuel_Price: Cost of fuel in the region**
**CPI: Consumer price index**
**Unemployment: Unemployment rate**
**MarkDown1, MarkDown2, MarkDown3, MarkDown4: Promotional markdowns**
**Dept: Department number**
**Size: Store size**
**Type: Store type (based on Size)**
## Tasks
1. Merge and Transform Data: Combine the data sources and perform data manipulations. Store the result in clean_data with the following columns:

**"Store_ID"**
**"Month"**
**"Dept"**
**"IsHoliday"**
**"Weekly_Sales"**
**"CPI"**
**"Unemployment"**
2. Analyze Monthly Sales: Calculate the average monthly sales and store the results in agg_data with columns:

**"Month"**
**"Avg_Sales"**
3.Save Results: Save clean_data and agg_data as CSV files.
