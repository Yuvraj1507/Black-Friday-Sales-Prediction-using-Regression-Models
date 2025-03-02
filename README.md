📊 Black Friday Sales Prediction using Regression Models 🚀



Project Overview 📈

This project aims to predict product purchase amounts during Black Friday sales using machine learning algorithms. By leveraging historical sales data, we aim to help retail stores optimize their product pricing strategies for maximum profit. Multiple regression models were implemented to forecast sales, and the best-performing model was selected based on evaluation metrics like RMSE.



🛠️ Technologies Used

Frontend:
Python
Jupyter Notebooks
Matplotlib, Seaborn (for data visualization)

Backend:
Pandas, NumPy (for data manipulation and preprocessing)
Scikit-learn, XGBoost (for machine learning models)

Tools:
Jupyter Notebook (for implementation and testing)
GitHub (for version control and collaboration)

![alt text](https://searchengineland.com/figz/wp-content/seloads/2014/12/black-friday1-ss-1920.jpg "Black Friday Sales Prediction")



⚙️ Key Features

Data Preprocessing: Cleaned the dataset by handling missing values and encoding categorical variables.

Exploratory Data Analysis (EDA): Analyzed consumer behavior, spending patterns, and demographic insights.

Model Building: Implemented and tuned multiple regression models, including Linear Regression, Decision Tree, Random Forest, and XGBoost.

Model Evaluation: Used Root Mean Squared Error (RMSE) as the evaluation metric to select the best-performing model.

Insights: Extracted valuable insights into customer behavior and spending patterns to help optimize pricing strategies.




## Table Of Contents
  - [Project Introduction](#project-introduction)
  - [Dataset Description](#dataset-description)
  - [EDA](#eda)
  - [Data Preprocessing](#data-preparation)
  - [Modeling Phase](#modeling-phase)
  - [Evaluation Metric](#evaluation-metric)
  - [Conclusion](#conclusion)

### Project Introduction
Black Friday is an informal name for the Friday following Thanksgiving Day in the United States, which is celebrated on the fourth Thursday of November. The day after Thanksgiving has been regarded as the beginning of the United States Christmas shopping season since 1952, although the term "Black Friday" did not become widely used until more recent decades. Many stores offer highly promoted sales on Black Friday and open very early, such as at midnight, or may even start their sales at some time on Thanksgiving. The major challenge for a Retail store or eCommerce business is to choose product price such that they get maximum profit at the end of the sales. Our project deals with determining the product prices based on the historical retail store sales data. After generating the predictions, our model will help the retail store to decide the price of the products to earn more profits.

### Dataset Description
The dataset is acquired from an online data analytics hackathon hosted by Analytics Vidhya. The data contained features like age, gender, marital status, categories of products purchased, city demographics, purchase amount etc. The data consists of 12 columns and 537577 records. Our model will be predicting the purchase amount of the products.

###  EDA:
Below are the observations which we have made from the data visualization done as part of the Data Understanding process.
* Approximately, 75% of the number of purchases are made by Male users and rest of the 25% is done by female users. This tells us the Male consumers are the major contributors to the number of sales for the retail store.On average the male gender spends more money on purchase contrary to female, and it is possible to also observe this trend by adding the total value of purchase.
* When we combined Purchase and Marital_Status for analysis, we came to know that Single Men spend the most during the Black Friday. It also tells that Men tend to spend less once they are married. It maybe because of the added responsibilities.
* For Age feature, we observed the consumers who belong to the age group 25-40 tend to spend the most.
* There is an interesting column Stay_In_Current_City_Years, after analyzing this column we came to know the people who have spent 1 year in the city tend to spend the most. This is understandable as, people who have spent more than 4 years in the city are generally well settled and are less interested in buying new things as compared to the people new to the city, who tend to buy more.
* When examining which city the product was purchased to our surprise, even though the city B is majorly responsible for the overall sales income, but when it comes to the above product, it majorly purchased in the city C.

### Data Preparation
* Used LabelEncoder for encoding the categorical columns like Age, Gender and City_Category
* Used get_dummies form Pandas package for converting categorical variable State_In_Current_Years into dummy/indicator variables.
* Filled the missing values in the Product_Category_2 and Product_Category_3

### Modeling Phase
- Splitted dataset into into random train and test subset of ratio 80:20
- Implemented multiple supervised models such as Linear Regressor, Decision Tree Regressor, Random Forest Regressor.

### Evaluation Metric
Root Mean Square Error (RMSE) is a standard way to measure the error of a model in predicting quantitative data. It’s the square root of the average of squared differences between prediction and actual observation.

### Conclusion
Implanted multiple supervised models such as Linear Regressor,Decision Tree Regressor, Random Forest Regressor and XGBOOST Regressor. Out of these supervised models, based on the RMSE scores XGBRegressor/XGBOOST Regressor was the best performer with a score of 2879.



📝 How to Run
Clone the repository to your local machine:
git clone https://github.com/your-username/black-friday-sales-prediction.git


Navigate to the project directory:
cd black-friday-sales-prediction


Install the required dependencies:
pip install -r requirements.txt


Open the Jupyter Notebook:
jupyter notebook


Run the notebook cells sequentially to see data processing, model building, and evaluation steps.



📊 Project Insights

Gender Analysis: The majority of purchases were made by male consumers.
Age Group Spending: Consumers between the ages of 25-40 spent the most during Black Friday.
City Demographics: City B had the highest overall sales, but specific products were predominantly purchased in City C.
Marital Status: Single men spent more than married men, potentially due to fewer financial responsibilities.

📈 Model Performance

Linear Regression RMSE: 3000
Decision Tree RMSE: 2800
Random Forest RMSE: 2900
XGBoost RMSE: 2879 (Best Model)
The XGBoost Regressor outperformed other models with the lowest RMSE, making
it the optimal choice for predicting sales amounts.



📚 Conclusion

This project demonstrates how machine learning can be applied to real-world business challenges like sales forecasting.
By predicting the purchase amount, retailers can make more informed decisions about 
pricing, inventory, and promotional strategies during the Black Friday sales period.

