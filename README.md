# Sales-Performance-Analysis
This project analyzes a sales dataset to extract critical insights, identify underlying trends, evaluate customer purchasing patterns, and deliver data-driven recommendations to enhance strategic decision-making and business performance.
### Project overview
The primary goal of this project is to analyze the company's sales performance and generate strategic insights by:
- Understanding total sales volume and revenue generation over time.
- Identifying the top-performing product categories and bestselling products.
- Analyzing regional sales patterns to pinpoint areas of strength and opportunity.
- Evaluating payment method preferences among customers.
- Discovering monthly seasonality and sales peaks.
- Providing data-driven recommendations to boost sales and improve marketing strategies.

![Screenshot 2025-04-28 102530](https://github.com/user-attachments/assets/db808916-29ca-4033-8835-ec4ab27a1eea)
### Dataset
The datset for this analysis consit of 240 rows and 10 columns some of which are;
- **Regions:** North America, Europe, Asia
- **Product Categories:** Electronics, Home Appliances, Clothing, Books, Beauty Products, and others
- **Product name**
- **Metrics Captured:** Units Sold, Unit Price, Total Revenue, Payment Methods, Regional Sales

Check out the dataset here [Sales Perfromance dataset](https://github.com/timiols/Sales-Performance-Analysis/blob/41bd295a70e3767e80dcc170f4564d8d28720c50/SALES%20PERFORMANCE.csv) 
### Tools
- Power BI
- Power Query
### Data Cleaning
The data came in a structured Csv format and hence didn't require deep cleaning, missing values were handled, columns changed inot proper data format and a couple of neccessary measures were created.
### Exploratory Data Analysis
Which product categories contribute most to total revenue?

![Screenshot 2025-04-28 115925](https://github.com/user-attachments/assets/bd531c28-3e89-41ea-bf24-7f85f8385a32)

Which region generates the highest revenue and sales volume?

![Screenshot 2025-04-28 115153](https://github.com/user-attachments/assets/d43a35c5-73c5-4764-be0f-e4e56075afc0)

How do monthly sales vary? Are there any noticeable seasonal trends?

![Screenshot 2025-04-28 120723](https://github.com/user-attachments/assets/2416d034-efbf-40a3-ba45-7222e26e72e3)

What payment methods are most popular among customers?

![Screenshot 2025-04-28 121305](https://github.com/user-attachments/assets/d14f3978-557c-43e3-8500-e6b9a4f8a93b)

Which products are the top sellers?

![Screenshot 2025-04-28 121442](https://github.com/user-attachments/assets/9a5f31db-1357-4eb5-b33b-3081acd39a9b)

### Data analysis
Power BI dax functions was used to create and insert relevant measures to enhance the useability of the dataset. Here are the queries deployed in this analyis:
```SQL
Average order value = [Gross revenue]/[Total transactions]
```
```SQL
Gross revenue = SUM(Sheet1[Total revenue])
```
```SQL
Total transactions = COUNT(Sheet1[Transaction ID])
```
```SQL
Total units sold = SUM(Sheet1[Units Sold])
```
### Results and Findings
- January being the highest grossing month suggests strong performance early in the year, likely tied to seasonal demand 
  (e.g.  post-holiday shopping or New Year promotions).
- Electronics dominate revenue, followed by home appliances and sporting goods. Beauty and books contribute marginally.
- North America is the leading region, contributing almost half of total revenue.
- Credit cards are by far the preferred payment method - used in over 60% of sales made.
- High-ticket electronics such as Canon EOS R5 Camera and LG OLED TV are leading revenue drivers, despite low unit sales.

Recommendation
-   Expand product offerings in Electronics category.
-   Explore Regional Growth in Asia and Europe by targeting marketing or localized promotions.
-   Offer Promotions in Off-Peak Months through discounts or marketing campaigns. This will Boost sales in months like July and
    August.
-  Diversify Payment Options by integrating other payment methods to reduce the dominance of credit cards.











