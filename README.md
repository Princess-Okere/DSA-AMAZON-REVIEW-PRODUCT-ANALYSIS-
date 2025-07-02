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
4. Data Formatting:Converted prices to currency format.
Used custom number formats (e.g., adding 'k' to reduce figure length).
5. Created Helper Columns:
Potential Revenue = Actual Price × Rating Count
Combined Score (for top-rated products) = Rating + (Rating Count / Scaling Factor)
Salary Band logic adapted for price range distribution.
