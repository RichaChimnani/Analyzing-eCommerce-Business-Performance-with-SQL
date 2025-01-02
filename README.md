# Analyzing-eCommerce-Business-Performance-with-SQL

Background Project
Measuring business performance is very important for every company. It will help you assess your current market, access new customers and find new business opportunities. This time, I will analyze business performance of an e-Commerce by reviewing it customer growth, product quality, and payment methods.

The dataset that will be used today was provided by Rakamin Academy. It has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions : from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. I will perform the analysis using PostgreSQL and create the visualization using Google Data Studio

Data Preparation
Before starting data processing, the first step that must be done is to prepare the raw data into structured and ready-to-process data. The following eCommerce dataset consists of 8 datasets that will interact with each other. So the steps taken are as follows:

Create a new database and its tables for the data that has been prepared by paying attention to the data type of each column.
Importing csv data into the database by paying attention to the dataset storage path.
Create entity relationships between tables, based on the schema in Figure 1. Data Relationship.
Then export the Entity Relationship Diagram (ERD) in the form of an image by setting the data type and naming the columns between interconnected tables.
image
Figure 1. Data Relationship

After adjusting the columns that are the primary and foreign keys in each dataset, the Entity Relationship Diagram (ERD) is generated as follows.
image
Figure 2. Entity Relationship Diagram

Annual Customer Activity Growth Analysis
The following is a table of combined results from the matrix between Number of Monthly Active Users, Number of New Customers per year, number of customers who make repeat orders per year, and the average frequency of orders every year. image
Figure 3. Overall Anuual Customer Activity Growth Analysis

image
Figure 4. Average Active User vs New Customer

There was a significant increase in 2017 because the data available in 2016 was only for the last 4 months, starting in September, so it can be concluded that there was only an increase in growth in 2017.
Meanwhile, the trend of Monthly Active Users (MAU) also increases every year, reaching 5,338 customers.
image
Figure 5. Repeat order vs Average Frequency Order

There was an increasing trend from 2017 to 2018 for the number of customers who made a purchase more than once. However, in 2018 there was a slight decrease in the number of customers who made purchases more than once.
The average number of orders made by customers does not change much each year, the average customer only makes 1 order.
Annual Product Category Quality Analysis
The following table shows the combined results of the matrix between the company's revenue, the number of canceled orders, the product category that gives the highest total revenue, and the product category that has the number of canceled orders each year. image
Figure 6. Overall Annual Product Category Quality

image
Figure 7. Best Selling Category Product and Revenue
By looking at the results on the side, we can see that the top sales / best selling product category is always change every year. There was also an increase revenue over the year.

image
Figure 8. Best Selling Category vs Most Cancelled Category
Most cancelled product category is always changing over the year. But for year 2018, interestingly, both most cancelled product category and best selling product category were health & beauty. This could be because health & beauty category was dominating overall transactions made in 2018.

Annual Payment Type Usage Analysis
The following is a table of information regarding the number of users of each payment type for each year. image
Figure 9. Overall Annual Payment Type Usage

image
Figure 10. Payment Type Usage per Year

Overall, the most preferred payment method is credit card. Further analysis can be done on customer behaviour in using credit card, such as the selected tenor, which product categories are usually purchased with a credit card, etc.
As for debit card, we can see that three was a significant increase from 2017 to 2018. On the other hand, voucher usage was decrease from 2017 to 2018.
It could be due to promotions/collaborations with certain debit cards as well as a reduction in promotional methods using vouchers. Further analysis can be done by confirming with other departments, for example marketing or Business Development regarding this.
Summary
From the aspect of customer growth or Annual Customer Activity Growth It can be said that the growth of new subscribers that occurred in 2017 was indicated by increasing the number of new customers and the number of Monthly Active Users (MAU).
On the other hand, there was a slight decrease in the number of customers who made purchases more than once in 2018.
The average number of orders by customer is only once.
Meanwhile, from the aspect of product quality or Annual Product Category Quality Analysis, there is an increase in the company's total revenue every year.
The product categories that get the most cancelled and the most selling orders change each year. But for year 2018, interestingly, both most cancelled product category and most selling product category were health & beauty.
In addition, the most popular type of payment from year to year is Credit Card.
