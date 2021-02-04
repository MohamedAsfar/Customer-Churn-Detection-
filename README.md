
# Customer Churn Detection 

![Churn](https://user-images.githubusercontent.com/68263684/106863485-d975ed80-6685-11eb-8af8-e44ce13f3e84.png)


---

### Table of Contents
You're sections headers will be used to reference location of destination.

- [Introduction](#Introduction)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Partition](#Data-Partition)
- [Feature Engineering](#Feature-Engineering)
- [Methods Used](#Methods Used)

---

## DEFINE

Customer Churn, also known as customer attrition, customer turnover, or customer defection, is the loss of clients or customers in the industry. Finance, Bank, Telecom and E-commerce companies use churn rate as their key performance metric in defining their success rate. The dollars spent on retaining existing clients is undeniably not as much as gaining another one. The analysis centers around the conduct of bank clients who are bound to leave the bank. The striking aspects of the customer behaviors are analyzed and visualized through Exploratory Data Analysis. Further, a Machine Learning model is created based on the customer who are likely to churn.

## DISCOVER

The Bank dataset is collected from Kaggle.com . The dataset consists of 10127 rows and 22 columns. The following table gives a description of the various numerical and categorical data.

| Variable  | Data type |
| ------------- | ------------- |
| Client Number  | Integer  |
| Attrition_Flag  | String  |
| Customer_Age  | Integer  |
| Dependent_count  | Integer  |
| Education_Level  | String |
| Marital_Status  | String  |
| Income_Category  | String  |
| Card_Category | String  |
| Months_on_book  | Integer  |
| Total_Relationship_Count  | Integer  |
| Months_Inactive  | Integer  |
| No of Contacts  | Integer  |
| Total_Revolving_Bal  | float  |
| Avg_Open_To_Buy  | float  |
| Total Transaction Amount  | float  |
| Total Transaction Count  | float  |
| Change in Transaction Count  | float  |
| Avg_Utilization_Ratio  | float  |
| Credit_Limit  | float  |


## EXPLORATORY DATA ANALYSIS

1. Exisitng VS Attrited Customers

![EDA 1](https://user-images.githubusercontent.com/68263684/106864030-98320d80-6686-11eb-817c-6742bc6ccc38.png)


## Data Partition

We partitioned our data into Training and Test sets. The training partition which is typically the largest partition was 75% of the main data frame and the test sets was 25% respectively. The main reason behind dividing the dataset into two parts was to check the accuracy of the model which is based on the test set. The division of the dataset is to minimize the concept of overfitting. An unbiased estimation of how well the model will do with new data will be given by applying the model to the test data that it has not seen before.

## Feature Engineering

Predictive Analytics use churn prediction models that predict customer churn by assessing their propensity of risk to churn. In order to do find the correlation between the different attributes, a correlation matrix is calculated. Feature Engineering should be performed by crating the correct dataset and choosing the right attributes. Since this problem is based on a binary value (0 or 1), a prediction model can be created based on Decision Tree, Random Forest, Logistic Regression and Artificial neural network which can diffuse multicollinearity. 

#### Methods Used

- Artificial Neural Network
- Random Forest
- Logistic Regression
- Decision Tree 

[Back To The Top](#Customer-Churn-Detection)

---

## Model Selection

| No  | Accuracy |
| ------------- | ------------- |
| Artificial Neural Network  | 93.48%  |
| Random Forest  | 94.91%  |
| Logistic Regression  | 90.62%  |
| Decision Tree  | 94.17%  |

## Conclusion

---

