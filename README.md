
# Customer Churn Detection 

![Churn](https://user-images.githubusercontent.com/68263684/106863485-d975ed80-6685-11eb-8af8-e44ce13f3e84.png)


---

### Table of Contents
You're sections headers will be used to reference location of destination.

- [Define](#Define)
- [Discover](#Discover)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Partition](#Data-Partition)
- [Feature Engineering](#Feature-Engineering)
- [Data Partition](#Data-Partition)
- [Methods Used](#Methods-Used)
- [Model Selection](#Model-Selection)
- [Conclusion](#Conclusion)

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

- Exisitng VS Attrited Customers

![EDA 1](https://user-images.githubusercontent.com/68263684/106864030-98320d80-6686-11eb-817c-6742bc6ccc38.png)

- Gender

![EDA 2](https://user-images.githubusercontent.com/68263684/106864406-0f67a180-6687-11eb-80d1-8a47a30171a0.png)

- Card Category

![EDA 4](https://user-images.githubusercontent.com/68263684/106864525-3b832280-6687-11eb-9be4-039991573571.png)

- Income Category

![EDA 5](https://user-images.githubusercontent.com/68263684/106864602-5786c400-6687-11eb-9407-a63516c7654a.png)

- Age Distribution

![EDA 6](https://user-images.githubusercontent.com/68263684/106864721-7edd9100-6687-11eb-8ad2-9caa796e160b.png)

- Months on book

![EDA 7](https://user-images.githubusercontent.com/68263684/106864798-961c7e80-6687-11eb-854b-abc79b44f58f.png)

- Eduaction Level

![EDA 9](https://user-images.githubusercontent.com/68263684/106864999-cf54ee80-6687-11eb-9aaf-872212a2a259.png)

### Points to Note

- Among 10127 customers, 1628 customers have left the bank which indicates 16.08% churn rate in the bank
- The credit cards are categorized into four groups namely Blue, Gold, Silver and Platinum with Blue being the most.
- The customers were more attracted during week 36 which denotes that the bank might have given extra coupons, gifts during this time
- Age is found to be normally distributed
- The higher they spend annually, the customers are more likely to remain
- After 2-3 months of inactivity, the customers are more likely to leave
- The higher the credit limit is, the customers are more likely to remain
- Almost all churned customers used their cards below 100 times

## Data Partition

We partitioned our data into Training and Test sets. The training partition which is typically the largest partition was 75% of the main data frame and the test sets was 25% respectively. The main reason behind dividing the dataset into two parts was to check the accuracy of the model which is based on the test set. The division of the dataset is to minimize the concept of overfitting. An unbiased estimation of how well the model will do with new data will be given by applying the model to the test data that it has not seen before.

## Feature Engineering

![FE 1](https://user-images.githubusercontent.com/68263684/106865893-07a8fc80-6689-11eb-93e1-13f8b85c0008.png)

Predictive Analytics uses churn prediction models that predict customer churn by assessing their propensity of risk to churn. To do find the correlation between the different attributes, a correlation matrix is calculated. Feature Engineering should be performed by creating the correct dataset and choosing the right attributes. Since this problem is based on a binary value (0 or 1), a prediction model can be created based on a Decision Tree, Random Forest, Logistic Regression, and Artificial neural network which can diffuse multicollinearity. Before that the categorical variables are converted into numerical varibables and Standard Scaling is done so that all the features contribute equally to the result

#### Methods Used

- Artificial Neural Network
- Random Forest
- Logistic Regression
- Decision Tree 



---

## Model Selection

| Model  | Accuracy | Precision Score | Recall Score |
| ------- | --- | --- |--- |
| Artificial Neural Network  | 93.48%  | 78.47%  | 76.69%  |
| Random Forest  | 94.91%  | 90.51%  | 74.43%  |
| Logistic Regression  | 90.62%  | 74.08%  | 59.22%  |
| Decision Tree  | 94.17%  | 81.93%  | 79.28%  |

## Conclusion

![Random Forest](https://user-images.githubusercontent.com/68263684/106872551-abe27180-6690-11eb-8d9c-c42807c37b6b.png)

From the above curve, it is clear that Random Forest is the most accurate model with an accuracy of 94.91%. 

---
[Back To The Top](#Customer-Churn-Detection)
