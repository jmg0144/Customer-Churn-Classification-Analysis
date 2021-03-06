# SyriaTel Customer Churn Analysis

## Overview
This project analyzes SyriaTel customer account data in order to build classifications models aimed at predicting customer churn. 
## Business Objective
SyriaTel, a telecommunications company, is interested in knowing the important factors in determining whether or not a customer will stay with the company. The primary goal of this notebook is to help SyriaTel keep current customers and offer business strategies on how to do so based on the analysis provided.  

## Data
The dataset contains relevant customer account data including:

  - The state of the customer.
    
  - The account length of the customer.
    
  - The customer's area code.
    
  - Whether or not the customer has an international plan.
    
  - Whether or not the customer has a voicemail plan.
    
  - The total day, evening, night, and international minutes of the customer.
    
  - The total day, evening, night, and international calls of the customer.
    
  - The total day, evening, night, and international charge of the customer.
    
  - The total customer service calls of the customer.
    
  - Whether or not the customer was 'true' or 'false' churn (true churn meaning that they have left the company, this will be the primary focus of the models).
  
  - The data contains no missing values.

![Screen Shot 2021-10-12 at 5 29 28 PM](https://user-images.githubusercontent.com/66973223/137032113-ee4ab177-ea09-490a-88b2-75942a2c066e.png)
 - Data contains significatly more 'false's than 'true's, this will need to be addressed later when building models in order to prevent class imbalance.

![Screen Shot 2021-10-12 at 5 30 06 PM](https://user-images.githubusercontent.com/66973223/137032197-4c16e344-a6ff-4009-b2af-c34d4b5820cc.png)
 - Internaional plan will need to be converted to a categorical feature.

![Screen Shot 2021-10-12 at 5 30 19 PM](https://user-images.githubusercontent.com/66973223/137032241-f790f235-7eec-41bb-9699-4ff578dd0a82.png)
 - Customer service calls does not appear to be evenly distributed. This feature could be relevant at predicting churn as cutomers who are unhappy with their service would likely make more customer service calls.

## Methods
* SyriaTel customer data will be used to create six different classification models to predict customer churn.

* The models will then be analyzed according to the precision metric.

* The best performing model will be analyzed for top feature importance.

* Business recommendations will then be presented. 

## Results & Conclusions
![Screen Shot 2021-10-12 at 7 35 40 PM](https://user-images.githubusercontent.com/66973223/137042873-202a3c36-4697-4bef-87eb-a32cafa073ef.png)

![Screen Shot 2021-10-12 at 7 15 41 PM](https://user-images.githubusercontent.com/66973223/137041678-44f948ea-d3fd-4d32-8c70-48added90f99.png)

![Screen Shot 2021-10-12 at 8 39 21 PM](https://user-images.githubusercontent.com/66973223/137047570-b9dafe95-b6d1-4dff-ade4-6377045a9d36.png)

![Screen Shot 2021-10-12 at 7 16 23 PM](https://user-images.githubusercontent.com/66973223/137041739-2c0f1955-42d0-4fc7-8028-11e0fd01781e.png)

![Screen Shot 2021-10-12 at 7 16 36 PM](https://user-images.githubusercontent.com/66973223/137041780-43fbd7f5-2831-4885-974e-93167d27bcff.png)

## Top Performing Model
The top performing model accorinding to the precision and ROC metrics was a Random Forest model using GridsearchCV in order to tune parameters. The top three features according to this model include:

1. Total Charge
2. Customer Service Calls
3. Total International Minutes

![Screen Shot 2021-10-12 at 7 16 49 PM](https://user-images.githubusercontent.com/66973223/137041812-425271eb-9281-4e06-9d19-2e62df834887.png)

![Screen Shot 2021-10-12 at 7 55 04 PM](https://user-images.githubusercontent.com/66973223/137044314-8f6c30e6-23eb-4544-ac28-577bc3b9cd6e.png)

## Model Comparison
![Screen Shot 2021-10-12 at 5 39 50 PM](https://user-images.githubusercontent.com/66973223/137032824-36860349-c232-4fac-acc2-35cd3932e7f4.png)

Based on the analysis, my main business recommendations are as follows:

1. Offer discounts/promotions to customers with higher than average total charge costs.

2. Offer discounts/promotions to customer who frequently call customer service. As well as improving customer service as a whole to better resolve issues. 

3. Create a competitive international plan to prevent international customers from leaving as well as attract more international customers overall.

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/jmg0144/churn-analysis-project/blob/main/SyriaTel-Customer-Churn-Analysis.ipynb)
