# Customer Churn Prediction
![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/26be9ff8-7bd7-4d3c-9b52-9b887b85fedf)

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

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/9b502a94-e947-4f03-ac78-dcb3a66d7baf)

### 2.2 Dataset Import and Dictionary

![](https://github.com/RandyAikins/Python_CustomerChurnPrediction/assets/128720674/dc51200e-f86a-4085-96d3-3da6fac94235)

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



