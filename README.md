# Customer Churn Prediction
![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/3464ec13-ee0a-414d-97df-b289229a44f3)

### 1.1 Introduction
ConnectTel Telecom Company is a leading global telecommunications company known for its innovative connectivity solutions. ConnectTel offer reliable voice, data, and Internet services, including mobile networks, broadband, and enterprise solutions. Serving both individuals and corporations, ConnectTel prioritizes exceptional customer service and advanced technology. With strategic partnerships and a customer-centric approach, they are reshaping the telecom industry and enabling seamless communication worldwide.

### 1.2 Problem
ConnectTel is confronted with a critical challenge: tackling customer churn, a formidable obstacle to its ongoing viability and expansion. Regrettably, the company's existing tactics for retaining customers lack precision and effectiveness, leading to the unfortunate departure of valuable clientele to rival companies.

### 1.3 Objective
To overcome this challenge, ConnectTel aims to develop a robust customer churn prediction system. The company seeks to accurately forecast customer churn and implement targeted retention initiatives. Reduce customer attrition, enhance customer loyalty, and maintain a competitive edge in the highly dynamic and competitive telecommunications industry.

### 1.4 Task
- Identify trends and patterns in customers leading to churning.
- Revenue lost due to customer churn.
- Build a machine learning model to predict customer churn.

---
## 2.0 Data Overview

### 2.1 Import of Python Libraries
Necessary Python libraries are imported for data analysis, visualization, data preprocessing, model building, and evaluation.

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/f180a8f4-d529-4057-83d3-fb93fd0c7ee0)

### 2.2 Dataset Import and Dictionary

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/35514978-5b6c-488b-9fca-0ab11921d4b2)

- CustomerID: A unique identifier assigned to each telecom customer, enabling tracking and identification of individual customers. 
- Gender: The gender of the customer, which can be categorized as male, or female. This information helps in analyzing gender-based trends in customer churn. 
- SeniorCitizen: A binary indicator that identifies whether the customer is a senior citizen or not. This attribute helps in understanding if there are any specific churn patterns among senior customers. 
- Partner: Indicates whether the customer has a partner or not. This attribute helps in evaluating the impact of having a partner on churn behavior. 
- Dependents: Indicates whether the customer has dependents or not. This attribute helps in assessing the influence of having dependents on customer churn. 
- Tenure: The duration for which the customer has been subscribed to the telecom service. It represents the loyalty or longevity of the customer’s relationship with the company and is a significant predictor of churn. 
- PhoneService: Indicates whether the customer has a phone service or not. This attribute helps in understanding the impact of phone service on churn.
- MultipleLines: Indicates whether the customer has multiple lines or not. This attribute helps in analyzing the effect of having multiple lines on customer churn.  
- InternetService: Indicates the type of internet service subscribed by the customer, such as DSL, fiber optic, or no internet service. It helps in evaluating the relationship between internet service and churn. 
- OnlineSecurity: Indicates whether the customer has online security services or not. This attribute helps in analyzing the impact of online security on customer churn. 
- OnlineBackup: Indicates whether the customer has online backup services or not. This attribute helps in evaluating the impact of online backup on churn behavior. 
- DeviceProtection: Indicates whether the customer has device protection services or not. This attribute helps in understanding the influence of device protection on churn. 
- TechSupport: Indicates whether the customer has technical support services or not. This attribute helps in assessing the impact of tech support on churn behavior.  
- StreamingTV: Indicates whether the customer has streaming TV services or not. This attribute helps in evaluating the impact of streaming TV on customer churn.
- StreamingMovies: Indicates whether the customer has streaming movie services or not. This attribute helps in understanding the influence of streaming movies on churn behavior. 
- Contract: Indicates the type of contract the customer has, such as a month-to-month, one-year, or two-year contract. It is a crucial factor in predicting churn as different contract lengths may have varying impacts on customer loyalty. 
- PaperlessBilling: Indicates whether the customer has opted for paperless billing or not. This attribute helps in analyzing the effect of paperless billing on customer churn. 
- PaymentMethod: Indicates the method of payment used by the customer, such as electronic checks, mailed checks, bank transfers, or credit cards. This attribute helps in evaluating the impact of payment methods on churn. 
- MonthlyCharges: The amount charged to the customer on a monthly basis. It helps in understanding the relationship between monthly charges and churn behavior. 
- TotalCharges: The total amount charged to the customer over the entire tenure. It represents the cumulative revenue generated from the customer and may have an impact on churn. 
- Churn: The target variable indicates whether the customer has churned (canceled the service) or not. It is the main variable to predict in telecom customer churn analysis.

### 2.3 Data Assessment and Wrangling
- The dataset is assessed for its shape, information on the columns and datatypes, statistical description, duplicates, and null values
- 11 rows with null values are dropped as they are very few and dropping them will not have any significant impact on the analysis and prediction
- Data points with incorrect labels in 'No phone service' and 'No internet service' are replaced with 'No'

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/4957faa6-4ebb-4abe-b1a7-ec12247135cc)

---
## 3.0 Exploratory Data Analysis (EDA)
In the EDA, the dataset is analyzed using univariate and bivariate techniques to identify patterns in customers' behavior and spending concerning churn. Some of the following were analyzed:
- Distribution of customer tenure and churn rate
- Distribution of monthly charges and how much is lost due to churn
- Demographic distribution of customers and its impact on churn
- Support services and their impact on churn
- Payment methods and contracts and their impact on churn

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/fd0e0b2f-ca46-4e4a-9a78-801807b790e4)
![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/95c32945-5425-4883-807c-d08c03eba3bf)
![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/8f0fe327-3286-447e-b430-934bf675f014)

---
## 4.0 Machine Learning

### 4.1 Data Preprocessing and Feature Engineering
The data preprocessing and feature engineering involve:
- Dropping the CustomerID feature
- Encoding categorical features into numerical using One Hot Encoder for the nominal features and Label Encoder for the ordinal features
- Segmenting the dataset into predictor variables (x) and target variable (y)
- Standardized the x features using the StandardScaler from Scikit-Learn
- Splitting the data into training and testing sets at a ratio of 0.7:0.3

### 4.2 Model Selection and Training
These 4 machine-learning algorithms are selected for the model building:
- Logistic Regression
- Naive Bayes
- Random Forest
- Support Vector Machines

The data is trained with selected algorithms via:
- Instantiating the algorithms
- Fitting the algorithms on the training sets
- Predicting results using the testing set

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/1d60a492-6f8e-437c-888d-4c3357b0e8da)

### 4.3 Model Evaluation
The models built are evaluated using the following metrics:
- Recall Score: this is the primary evaluation metric as it measures the models' ability to identify churned customers correctly among actual churn
- Precision Score: this is a secondary metric that measures the models' ability to identify churned customers (true positive) among positive predictions
- F1 Score: this evaluation metric measures the harmony between the recall score and the precision score
- Accuracy Score: this evaluation metric looks at the overall ability of the model to correctly identify actual churn (true positive) and actual no churn (true negatives)

||LogisticRegression|NaiveBayes|RandomForest|SVM|
|---|---|---|---|---|
|Recall_Score|53.12%|73.44%|46.88%|46.88%|
|Precision_Score|63.81%|53.44%|61.74%|64.78%|
|F1_Score|57.98%|61.86%|53.29%|54.40%|
|Accuracy_Score|79.53%|75.92%|78.15%|79.10%|

### 4.4 Hyperparameters Tuning
Grid Search is used in adjusting the hyperparameters of the various algorithms to optimize their performance on the dataset. The scoring metric in the grid search is Recall_Score; hence, the algorithm's hyperparameters with the best score are selected for the final model building.

||best_score_|best_params_|
|---|---|---|
|LogisticRegression|0.6491368173810923|'C': 0.001, 'penalty': 'l2', 'solver': 'liblinear'|
|NaiveBayes|0.7760657662947739|'var_smoothing': 1.0|
|RandomForest|0.5314092777451556|6'max_depth': 10, 'n_estimators': 150|
|SVM|0.5421374045801526|'C': 1, 'gamma': 'scale', 'kernel': 'linear'|

### 4.5 Building and Evaluating Model using Naive Bayes (tuned hyperparameter)
Upon tuning the hyperparameters of all algorithms, Naive Bayes gives the best possible recall score of 0.7761 and is therefore selected for the customer churn prediction model.

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/e9c5228b-3e1b-44af-91a9-883202c822b5)
![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/f61123c9-16ab-43e5-8905-09c170ab88e0)

The customer churn prediction system has a Recall_Score of 78%. That is out of every 5 churn customers the system can identify about 4 of them correctly.

---

## 5.0 Conclusion

### 5.1 Task
In this Project, I set out to understand the customer churn challenge of ConnecTel which is posing an existential threat to the business, and also build a robust customer churn prediction system. From this, the following questions are to be answered:
- What are the trends in customers who are churning out of ConnectTel's business?
- How much revenue is ConnectTel losing due to customer churn?
- How best can churn be managed by leveraging machine learning tools to build a churn prediction system?


### 5.2 Insights 
1. Customer Churn Rate: ConnectTel has a churn rate of 26.6%, resulting in the loss of approximately 3 out of every 10 customers.
2. Revenue Impact: Customer churn leads to a loss of around 1/3 of the monthly recurring revenue, which amounts to $139,130.85. Churn is more prevalent among high-paying customers than low-paying ones.
3. Customer Tenure Distribution: The majority of ConnectTel's customers fall into two groups: very new and very old. Churn is higher among new customers compared to old customers.
4. Contract Length: Customers with month-to-month contracts are around 8 times more likely to churn than those on longer-term contracts (1 year or 2 years).
5. Payment Methods: Churn is higher among customers using Electronic Check for payment compared to customers using automatic payment methods.
6. Demographics: Gender has minimal impact on churn, with customers evenly distributed between genders. However, churn is proportionally higher among senior citizens. Churn is lower among partnered and dependent customers.
7. Phone and Internet Services: Phone service has a minimal impact on churn, regardless of whether customers have it or not. In contrast, customers using Fibre Optic internet service exhibit a significantly high churn rate of over 70%, surpassing DSL and no internet service.
8. Support Services: Customers who access support services like Online Security, Online Backup, Device Protection, and Tech Support experience lower churn rates compared to those without such services.

### 5.3 Retention Initiatives
1. More customers should be tied to longer-term contracts.
2. Customers should be incentivized to use automatic payment methods of bank transfer and credit card.
3. Some packages should be developed along customer demography to boost retention in SeniorCitizens, No Partner, and No Dependents customers.
4. Targeted packages should be made for customers using Fibre Optic internet service.
5. Customers should be incentivized to subscribe to support services.

### 5.4 Prediction System
A robust customer churn prediction system has been developed for ConnectTel using the Naive Bayes algorithm with other machine learning techniques such as:
- Data Preprocessing and Feature Engineering
- Exploratory Data Analysis
- Model building, Tunind, and Evaluation

The churn prediction system has a recall score of **78%, that is it identifies approximately 4 of every 5 churning customers** which will help reduce churn and revenue loss.
