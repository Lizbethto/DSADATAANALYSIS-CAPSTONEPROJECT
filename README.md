# DSADATAANALYSIS-CAPSTONEPROJECT
# Table of Contents
#### Project Overview
#### Project Files
#### Tools Used
#### Data Cleaning Steps
#### Pivot Table Analysis
#### Dashboard Preview
# Project Overview
##### This project presents a data analysis solution using Amazon Case Study. Tasked with analysing product and customer review data to generate insights that can guide product improvement, marketing strategies, and customer engagement.
### Objectives:
#### Data cleaning.
#### Create interactive PivotTable-based dashboard.
#### Derive insights from sales by using Discount Percentage, Price Range, Potential Revenue, and Rating × Review Score.
# Project Files
#### Amazon_case_study.xlsx -  Raw data file
#### Amazon_case_study.xlsx - cleaned file
#### Amazon_case_study.xlsx -	Interactive dashboard with PivotTables
# Tools Used
#### Microsoft Excel
#### PivotTables
#### PivotCharts
#### GitHub
# Data Cleaning Steps
#### Created another sheet called clean sheet
#### Removed duplicates using Product name.
#### Turned the file to Table
#### Cleaned the product name and category using =TRIM and =PROPER() function
#### Extracted new columns (e.g., Price Range).
#### Standardized text formatting (Product Categories, Product name).
# Pivot Table Analysis and calculated columns
## Q1: What is the average discount percentage by product category?
#### Rows → category Values → discount_percent → set to Average value is formatted as Percentage
##  Q2: How many products are listed under each category?
#### Rows → category Values → product_name → set to Count
## Q3: What is the total number of reviews per category?
#### Rows → category Values → review_count → set to Sum
## Q4: Which products have the highest average ratings?
#### Rows → product_name Values → rating → set to Average. Sort by Descending value
##  Q5: What is the average actual vs discounted price by category?
#### Rows → category Values:actual_price → set to Average 
### discounted_price → set to Average
##  Q6: Which products have the highest number of reviews?
#### Rows → product_name Values → review_count → set to Sum
#### Sort Descending by review count
## Q7: How many products have a discount of 50% or more?
### Using =COUNTIF([discount_percent],">=0.5") function
##  Q8: What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?
#### Rows → rating Values → product_name → Count
#### Sort rating in Ascending order
## Q9: What is the total potential revenue (actual_price * rating_count) by category?
#### Rows → category Values → potential_revenue → set to Sum. This as been Formatted as Currency
## Q10: What is the number of unique products per price range bucket (<₹200, ₹200–₹500, >₹500)?
#### Rows → price_range Values → product_name → Count
## Q11: How does the rating relate to the level of discount?
#### Rows → rating (rounded, if too granular) Values → discount_percent → Average
## Q12: How many products have fewer than 1,000 reviews?
#### Using =COUNTIF([review_count],"<1000") Function
##  Q13: Which categories have products with the highest discounts?
#### Rows → category Values → discount_percent → Max
## Q14: Identify the Top 5 Products in terms of rating × review score
### Rows → product_name Values → rating_review_score → Sum
#### Sort in Descending order and Use the filter to select Top 5
# Dashboard Preview


