# SkincareCompany
This project uses the D2C Skincare E-commerce Analytics dataset from Kaggle. The data analysis explores a skincare e-commerce synthetic dataset with multiple data tables to inform business decisions.

Files used:
- orders.csv
- items.csv
- products.csv
- reviews.csv
- returns.csv

## Tools Used
* Python
* Jupyter Notebook
* SQL(SQLite)
* Matplotlib
* Tableau

## Data Cleaning
* Confirmed data types were appropriate for each column.
* Verified there were no duplicated records found in each table.
* Checked over missing values in each table using isnull().sum() and only found one column (delivery_date) with missing values.
* Left the missing "delivery_date" values as these were not relevant to this analysis.
* Confirmed that column headers across the different tables were consistent.
* Later standardized values during exploratory data analysis for "skin_type" in products table to show consistently (Sensitive / Dry and Dry / sensitive to Dry / sensitive)

## SQL Analysis
### Most and Least Purchased Products

<img width="470" height="432" alt="image" src="https://github.com/user-attachments/assets/b87467e6-7d3b-471f-a0fa-e2820d1bb6c7" />

This query identify categories that are leading in purchases in the company by summming units purchased across the different categories (serums, moisturizers, sunscreen, etc). When it come to skincare category, serums (919 units) are contributing the most to sales followed by moisturizers (443 units) and sunscreen (314).

### Most and Least Rated Products
<img width="700" height="400" alt="image" src="https://github.com/user-attachments/assets/424eec92-0d12-4f1c-908a-324cf077d0df" />

This query identifies average ratings across the different categories of products sold by the company by averaging the the ratings for each category. Overall, D2C's ratings range from 3.7 to 4.1 out of a max rating of 5. 

### Driving Factor for Returns
<img width="2218" height="1402" alt="image" src="https://github.com/user-attachments/assets/f5c57c41-a617-4d49-9164-ef8aa963ae32" />

<img width="544" height="392" alt="image" src="https://github.com/user-attachments/assets/30ad1307-f24b-48a5-afae-7ab9d0b4f694" />


This query and matplotlib identify and visualize the return reasons and amount of returns made for each product as well as identifying the most common return reasons. The two most common reason of returns have to do with skin irritation and shipping complications including late deliveries (16) and damaged packaing (13) and the wrong item recieved. The total count for these summed return reason involving shipping is 29 followed by skin irritation with 28 returns. 

### Customers

### Regions and Acquisition Channels Driving Customers

### Revenue 
## Dashboard

https://public.tableau.com/views/SkincareWorkbook3/SkincareCompany?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Key Findings

## Recommendations
