# Car-Price-Prediction 

 ### Problem Statement:

To sell/buy a second-hand car the most important thing is to find the ideal price of the car. By getting the features of the car we can predict its ideal price using ML Models.
Online platforms which are used to sell second hand cars collects various information of cars. We will use these features in our model to predict car price.

### Dataset and Pre-Processing:
For this project, we are had scrapped the data from CarTrade (https://www.cartrade.com/ ) on used car sales for 40 different locations, the features available in this dataset are name, price, km, owner, year, fuel, location.

For each and every feature we removed irrelevant characters individually and then we bifurcate name feature into company name and model name
Outlier treatment: We removed high value cars such as 'Audi', 'BMW', 'Mercedes-Benz'. 

One-Hot Encoding: We converted the 'owner', 'carName', 'fuel', 'Company', 'location' into dummy variables

### Methodology:
We have used various regression model to predict car price such as:
•	Huber Regression technique that is robust to outliers. The idea is to use a different loss function rather than the traditional least-squares.

•	Random Forest Regressor is a supervised learning algorithm that uses ensemble learning method for regression. Ensemble learning method is a technique that combines predictions from multiple machine learning algorithms to make a more accurate prediction than a single model.

•	Extreme Gradient Boosting (XBG) it is an implementation of gradient boosting trees algorithm. It builds one tree at a time unlike random forest. This additive model (ensemble) works in a forward stage-wise manner, introducing a weak learner to improve the shortcomings of existing weak learners.


### Results:

Huber regression RMSE = 252618 R2Score = 0.75

RFG RMSE = 156862 R2Score = 0.90

XGB RMSE = 1288374 R2Score = 0.94

### Conclusion:

Compared to Random Forest Regressor, Huber Regression method did not perform comparably well. However Random Forests tend to overfit the dataset. Building up from the relatively good performance of XGB Regressor Method produced the best R2 Score on data. 
