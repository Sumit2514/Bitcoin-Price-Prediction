# Introduction:

Bitcoin has been increasingly regarded as an investment asset.Bitcoin’s value 
reflects investors’ confidence in cryptocurrency.Because of its highly volatile 
nature, there is a need for good predictions on which to base investment decisions. 
Existing studies have leveraged machine learning for more accurate Bitcoin price 
prediction, few have focused on the feasibility of applying different modelling 
techniques to samples with different dimensional features.

# Motivation:

Previous works simply concentrates only on accuracy when applying machine learning
algorithms without considering the sample dimension.Applying machine learning 
without considering sample dimension causes overfitting problem.Stock market 
prediction using daily data and accessible high-frequency data has grown over 
decades.Predicting Bitcoin price in similar manner is lacking

# Objective:

Leveraging appropriate Machine learning algorithms based upon characteristics of
sample and dimension to predict Bitcoin price

# Methodology:

Features for prediction models of Bitcoin daily price are : 
Block Size, Hash Rate, Mining Difficulty, Number of Transactions, Confirmed 
Transactions per Day, Mempool Transaction Count,  Mempool Size, Total Transaction 
Fees, Market Capitalization, Estimated Transaction Value, Time between blocks, 
Trades per minute, Google trend search volume index, and Gold spot price.


Features for prediction models of 5-minute interval Bitcoin trading price are :
Price, Trading Volume, Open, Close, High and Low points 

After apply wrapper method (backward elimination ) on Bitcoin daily price data 
for features selection . Following 12 features are selected for prediction models
 :Block Size, Hash Rate, Mining Difficulty, Number of Transactions, Confirmed 
Transactions per Day, Mempool Size, Mempool Transaction Count,Market Capitalization, Estimated Transaction Value, Total Transaction Fees, Google Trend Search Volume Index, and Gold Spot Price


For Bitcoin 5-minute interval price prediction model, feature data for tick 
trading data are poor or unavailable for very small intervals. Therefore, this  
paper consider the original features, which include Open, High, Close, Low, 
Price and Volume

# Implementation:

Develops a binary classification algorithm to predict the sign change of Bitcoin price

Binary dependent variables denoted as y ∈ { -1,1}. Here y = -1 indicates that the Bitcoin price drops while y= 1 indicates that the Bitcoin price increases.

Machine Learning Techniques used:

Logistic Regression
Linear Discriminant Analysis
Random Forest
Xgboost
Quadratic Discriminant Analysis
Support Vector Machine
Decision Tree
K-Nearest Neighbors

# Result:

Logistic Regression and Linear Discriminant Analysis performs better for daily data with high-dimensional features

XGBoost outperform other machine learning models for high-frequency data


