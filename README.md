**1. Context**

The telecommunications (telco) industry has developed rapidly in the 20th century. There are so many companies have been working in this business sector. Therefore the competition is always going to be there. Because of this high competition, telco companies have always improved and evaluated their service quality to succeed and not be taken over by competitors.

Customers are the most important asset for a company. It is the main focus of the business. A company usually puts in a big effort to get customers in the initial phase of building the company. Only After they gain the customer's trust, their business can continue to live on. But the work continues beyond there. They have to keep their existing customers to continue using their service and it is a challenging task.

Customer churn is a customers stop using a service, either they don't need the service anymore or they change to another service provider. Acquiring a new customer is far more expensive than retaining the existing ones. Even an [article](https://mailchimp.com/resources/customer-churn/) says that *"Acquiring a new customer can cost a business 5x more than retaining an existing one"*. Therefore, customer churn is a critical factor for sustaining long-term profitability.

**2. Problem Statement**

In order to keep their customers, telco company usually have plenty of prevention strategies such as personalized offers, customer engagement, feedback mechanism, and much more. A company usually allocate a budget to do these campaign. It is crucial to manage this budget, so it gets into the right hands. 

In this modern era, data has become an essential part of the business. Data can provide a lot of benefit to the company. It can help a company to understand their customers and condition around them. Also it can help company to spot a potential customer churn. By targeting the right customers, the company can maximize their budget by allocating it to the customers that potential to churn.

In this project we will use historical data of certain telco company consisting of almost 5000 rows and 11 columns with column that state if the customer is churning or not. This project aim to identify current customers who's likely to churn by loking at historical data. **A predictive solution leveraging data analytics and machine learning** can help us to identify these at-risk customers and optimize promotional strategies.

**3. Goal**

The purpose of this project are to:
- Analyze factors that influence a customer to churn
- Make a machine learning model to predict whether a customer will churn or not
- Deploy the corresponding model to cloud

**4. Analytical Approach**

We will take a look at the data by doing some exploratory data analysis (EDA) in hope to uncover the truth that still yet to be uncovered. By looking at several information provided from the data that might potentially have a correlation with churning customers. In the end, we will make several action recommendation based on insight being spotted while doing the data analysis process.

**5. Metric Evaluation**

Here we define the positive class as a churn customers with this detail.
- False Positive (FP): Predict a customer will churn, while it is not
- False Negative (FN): Predict a customer will not churn, while it is churn

Giving false prediction will result in these costs.
- FP cost: Waste of promotional budget
- FN cost: Lost of customers

This projects aims to spot as many potential churn as possible. We knew that acquiring a new customer is far more expensive than retaining the existing ones. Recall will be the metric that suit our interest. But, because we want to maximize the budget that are going to be spend to offer promotions to customers. We are going to take a little bit of concern to the model precision. 

To have a good measure of this, we will use the **F2-score** that give specific weight (2:1) to recall and precision. To better understand this metric, take a look at the equation below (Betha=2)
