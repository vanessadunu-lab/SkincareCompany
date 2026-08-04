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
<img width="1998" height="1598" alt="image" src="https://github.com/user-attachments/assets/5db93138-6253-4b6b-a8b9-161293a46d3a" />

https://public.tableau.com/views/SkincareWorkbook3/SkincareCompany?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Key Findings

The most purchased category of skincare products were serums (919 units purchased) followed by moisturizers (443 units purchased), and sunscreen (314 units purchased). The least purchased category is the toners (80 units purchased) followed by lip care (82 units purchased). 
The most purchased type of skincare was alpha arbutin serum for pigmentation (166 units purchased) followed by niacinamide serum (144 units), SPF 60 sunscreen (138 units), and hyaluronic acid serum for hydration (132 units). The least purchased was an alcohol free toner (34 units), multi-peptide eye cream for anti-ageing (39 units), and rose water hydrating toner (46 units).
RATINGS: The two products with the highest rating are: Vitamin B5 moisturizer (4.5) and PHA 3% Alcohol-free toner (4.43). The two products with the lowest rating are: Body Wash with Salicylic Acid (3.25) and Anti-Dandruff Shampoo for dandruff control (3.28).¶
CUSTOMERS: Maharashtra, Gujarat, and Madhya Pradesh are the top leading states when it comes to driving clientele. This could inform how acquisition channels are distributed towards different states in order to increase clientele.
MONEY: 5% AND 10% discounts brought in the most revenue compared to the original pricing or higher discounts like 20% and 25%. Prioritizing 5% and 10% discounts over larger discounts initially may help to increase revenue from the products. Based on category and including discounts also helping to drive purchases, serums are leading with 919 units purchased and 540249.75, moisturizers with and 443 units purchased and 155518.60, and sunscreen with 129390.00 rupees. The 5% discounts brought in 307000.1 rupees leading in purchases and revenue followed by 10% with 595 units purchased and revenue of 273694.5 rupees, and 0% with 487 units purcahsesd and 241113 rupees in revenue.

## Recommendations
