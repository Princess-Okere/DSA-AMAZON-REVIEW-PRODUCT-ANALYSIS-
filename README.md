# DSA-AMAZON-REVIEW-PRODUCT-ANALYSIS-
 This project was completed as part of a Data Analysis course at Digital Skillup Africa (DSA). It involves cleaning, exploring, and analyzing an Amazon product dataset using Microsoft Excel, with additional visual insights presented through pivot tables, charts, and a dashboard.
Key analysis includes product pricing trends, customer review distribution, discount patterns, and top-performing categories.


## Dataset Description
The dataset includes information scraped from Amazon product pages and contains the following features:
Product Name
Category
Actual Price
Discounted Price
Discount Percentage
Rating Count
Average Rating
These variables provide both numerical and categorical insights into product pricing, discounting, popularity, and customer feedback.

## Data cleaning steps
The following steps were carried out to prepare the data for analysis:
1. Structured Table Format: The dataset was converted into a structured Excel table to support dynamic referencing
2. Whitespace Removal: Trimmed all leading/trailing spaces across all columns
3. Missing Values: Checked for and cleaned cells with missing or irrelevant data (especially in Rating Count and Category).
4. I checked for duplicates in the datasets, checked also for blank spaces and identied one(H284).
5. I selected the headers of my column and made it bold using ctrl+shift+down arrow. proceeded to increase the font of my header amd capitalized the first letter of the header names.
6. I did use the find and replace tool to get rid of extra spaces and unprintable characters. 
7. Data Formatting:Converted prices to currency format. Used custom number formats (e.g., adding 'k' to reduce figure length).
8. Created Helper Columns:
Potential Revenue = Actual Price × Rating Count
Combined Score (for top-rated products) = Rating + (Rating Count / Scaling Factor)
Salary Band logic adapted for price range distribution.

## Visualization
Each question in the case study was tackled with a mix of Pivot Tables, Charts, and Text Boxes for insights. 
NOTE: These insights are in the excel file uploaded to this repository.
Each of the 14 analysis tasks was tackled using Pivot Tables, COUNTIF functions, calculated columns, and charts. The visualizations were built on a dashboard worksheet, with text boxes added for clear interpretation and slicers used for interactivity in selected cases.

1. Average Discount Percentage by Product Category
Chart Type: Bar Chart
Method: Pivot Table with Average of Discount
Interpretation: Identified which categories offer the highest average discounts.

2. Number of Products per Category
Chart Type: Bar Chart (Top 10 filter applied)
Method: Pivot Table using count of products
Interpretation: Revealed the most populated categories in the dataset.

3. Total Number of Reviews per Category
Chart Type: Bar Chart (entire dataset)
Method: Pivot Table with sum of Rating Count
Interpretation: Helped identify categories receiving the most user engagement.

4. Products with the Highest Average Ratings
Chart Type: Column Chart
Method: Filtered Pivot Table showing products with top average ratings (e.g., 5.0)
Interpretation: Showed user-favorite products based on rating alone.

5. Average Actual Price vs. Discounted Price by Category
Chart Type: Clustered Column Chart
Method: Pivot Table with two average fields (actual price, discounted price)
Enhancement: Data labels were formatted with custom 'k' values (e.g., ₹5k)
Interpretation: Compared standard vs. discounted pricing strategies.

6. Products with the Highest Number of Reviews
Chart Type: Bar Chart
Method: Pivot Table sorted by descending rating count
Filter: Top 1 product only
Interpretation: Pinpointed the product with the most user reviews.

7. Products with 50% or More Discount
Display Type: Pivot Table (Top 15)
Method: Filtered on products where discount ≥50%
Interpretation: Showed most discounted items, likely for promotions or clearance.

8. Distribution of Product Ratings
Chart Type: Bar Chart
Method: Pivot Table using average rating grouped
Color Coding: Red = highest frequency, Green = least
Interpretation: Most products fell within 4.0–4.5 range, showing high customer satisfaction.

9. Potential Revenue by Category
Chart Type: Bar Chart
Method: Calculated Column (actual_price * rating_count) → summarized in Pivot Table
Format: Custom values displayed in ₹k or ₹bn
Interpretation: Some high-volume low-priced products generated more potential revenue.

10. Unique Products per Price Range
Chart Type: Pie Chart
Price Ranges: <₹200, ₹200–₹500, >₹500
Method: COUNTIF with buckets
Interpretation: Majority of products were priced above ₹500.

11. Rating vs Discount Correlation
Chart Type: Scatter Plot with Trendline
Method: Two-axis chart using rating and discount
Interpretation: No strong correlation observed; high discounts don’t always mean poor ratings.

12. Products with Fewer Than 1,000 Reviews
Display Type: Text Box only
Method: =COUNTIF([Rating Count], "<1000")
Value: 326 products
Interpretation: A significant portion of items have limited reviews, indicating low user engagement or new listings.

13. Categories with the Highest Discounts
Chart Type: Bar Chart
Method: Pivot Table with average discount per category
Filter: Top 8 categories
Interpretation: Highlighted discount-heavy categories likely used for sales strategy.

14. Top 5 Products by Rating + Number of Reviews Combined
Chart Type: Column Chart
Method: Calculated column: Average Rating + (Rating Count / 1000) → sorted
Pivot Table: Used to extract top 5 products
Interpretation: Balanced metric combining popularity and satisfaction.

## Conclusion
This Amazon Product Review Analysis project provided valuable hands-on experience in applying core Excel data analysis techniques to extract insights from a real-world dataset. By answering 14 targeted business questions, I was able to build a clean, interactive dashboard that highlights key metrics around product ratings, discounts, pricing, and customer engagement.
## key Learnings:
1. Pivot Tables are powerful for summarizing and slicing data efficiently, especially when working with large datasets.
2. Calculated Columns and formulas like COUNTIF helped derive new insights beyond the raw data.
3. Chart Selection Matters: Choosing the right chart types (e.g., clustered column, pie chart, scatter plot) significantly affects how clearly insights are communicated.
4. Filtering and Slicers enhance dashboard interactivity, allowing users to focus on the most relevant data (e.g., top categories or discount levels).
5. Custom Formatting (e.g., “₹k”) makes numerical data cleaner and easier to read, improving dashboard aesthetics and understanding.
6. Data-Driven Storytelling: Turning raw data into actionable insights required not just analysis, but also thoughtful interpretation, formatting, and organization for a non-technical audience.

