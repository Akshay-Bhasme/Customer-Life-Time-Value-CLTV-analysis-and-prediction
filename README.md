# Customer-Life-Time-Value-prediction
## CLTV: Customer Lifetime Value
Organizations invest in customers: acquisition cost, offline ads, promotions, discounts etc.

Customer Life time Value is the total worth to a business of a customer over the whole period of their relationship.

Lifetime value is an important metric as it costs less to keep existing customers than it does to acquire new ones, so increase the lifetime value of your existing customers is a great way to drive growth.

### Multiple Approaches:

- Using the following equation: CLTV = ((Average Order Value x Purchase Frequency)/Churn Rate) x Profit margin.
- Customer Value = Average Order Value * Purchase Frequency
- Average Order Value(AOV) = Total Revenue / Total Number of Orders. AOV represents the mean amount of revenue that the customer spends on an order.
- Purchase Frequency = Total Number of Orders / Total Number of Customers. It represents the average number of orders placed by each customer.
- Churn Rate: Churn Rate is the percentage of customers who have not ordered again.
- Customer Lifetime = 1/ churn rate
- Churn Rate= 1-Repeat Rate

Reference: https://towardsdatascience.com/measuring-users-with-customer-lifetime-value-cltv-94fccb4e532e
- CLTV can also implement using RFM(Recency, Frequency, Monetary) values.
- Lifetime value= Total Gross Revenue - Total cost

This equation now gives us the historical lifetime value.

### RFM Score: Recency, Frequency, Monetary value.
- Recency: How recently a customer has made a purchase

- Frequency: How often a customer makes a purchase

- Monetary Value: How much money a customer spends on purchases

A marketing analysis tool used to identify a firm's best clients based on the nature of their spending habits.
Evaluates clients and customers by scoring them in three categories: how recently they've made a purchase, how often they buy, and the size of their purchases.
Helps firms reasonably predict which customers are likely to purchase their products again, how much revenue comes from new (versus repeat) clients, and how to turn occasional buyers into habitual ones.
RFM scores for each customer ID are the perfect candidates for feature set.

- Low Value: Customers who are less active than others, not very frequent buyer/visitor and generates very low - zero - maybe negative revenue.
- Mid Value: In the middle of everything. Often using our platform (but not as much as our High Values), fairly frequent and generates moderate revenue.
- High Value: The group we don’t want to lose. High Revenue, Frequency and low Inactivity.

### Data:  
customer_segmentation data. (E-Commerce data available on Kaggle)

https://www.kaggle.com/code/fabiendaniel/customer-segmentation/data 

It has 8 features:

InvoiceNo: Unique Invoice Number, (Integer)

StockCode: Product(item) code, (Integer + Text)

Description: Description of the product, (Text)

Quantity: Purchased quantity of the product, (Integer)

InvoiceDate: Date of the Invoice, (dd/mm/yyyy)

UnitPrice: Price of the single unit of the product, (Float)

CustomerID: Unique Customer ID, (Integer)

Country: Name of the country. (Text)

### Approach:
We are going to build a simple machine learning model that predicts customers lifetime value.

#### Lifetime Value Prediction
- Define an appropriate time frame for Customer Lifetime Value calculation
- Identify the features we are going to use to predict future and create them
- Calculate lifetime value (LTV) for training the machine learning model
- Build and run the machine learning model
- Check if the model is useful
