# Time-Series-Forecast-Amazon-Halloween-Sales

In this notebook, I'm going to examine a few models for time series forecasting, in order to predict the demand for our Halloween products on Amazon.

Models: SARIMAX, GAM, Prophet, Linear Regression, Lasso, Ridge, ElasticNet, KNN, SVR, Decision Tree, Random Forest and XGBoost.

###Selling, Storing and Shipping via Amazon:

In the Amazon E-commerce business there are 2 options to store and deliver the products to the customers:
1. Upload the product on Amazon for sale but store it in your warehouse and take care of the shipping by yourself.
2. Send an inventory to Amazon, and Amazon takes care of the storage and the delivery directly to the customers.

In the second choice, Amazon takes an extra fee for that service but also gives a priority for these products and shows these lists in a better place on the page.

Sending stock to Amazon can provide a great potential of selling more merchandise and increase seller profits, but with that opportunity come risk. Sometimes the product is seasonal and if you don't succeed in selling it on time you are stuck with overstock which no one will buy until next year and you actually need to get rid of the stock and therefore lose money.

###The Task:

The task is to send stock to Amazon, stock of products for Halloween, and it needs to be sent 2 months before the event ends (31/10). 
Therefore we need to predict the total sales 2 months ahead.
Even though the data contains observations from 2021, the forecast period we trying to predict is the Halloween accrue at 2020 (31/10/2020) which will be the test set. 


###The Data:

The data I have got is a daily sales (quantity) for products tagged as Halloween products. These univariate time series contain quantities and dates (as index) from 2015 until 2021. I won't share because of confidential issues.

In addition, there is a table of holidays and their dates of each year (in this case we are using Halloween only).

###Table of Contents:

- Packages
- Helper Functions
- Quick EDA
- Holt-Winters Exponential Smoothing
- SARIMAX Model
- GAM - General Additive Model
- Facebook Prophet Model
- Classic ML Models
- Evaluation and Comparison
