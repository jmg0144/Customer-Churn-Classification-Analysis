# SyriaTel Customer Churn Analysis
Author: Justin Giovatto
## Overview
This project analyzes SyriaTel customer account data in order to build classifications models aimed at predicting customer churn. 
## Business Problem
SyriaTel, a telecommunications company, is interested in knowing the important factors in determining whether or not a customer will stay with the company. The primary goal of this notebook is to help SyriaTel keep current customers and offer business strategies on how to do so based on the analysis provided.  

## Data
The dataset contains relevant customer account data including:
  - The state the customer is from
    
  - The account length of the customer
    
  - the customer's area code
    
  - Whether or not the customer has an international plan
    
  - Whether or not the customer has a voicemail plan
    
  - The total day, evening, night, and international minutes of the customer
    
  - The total day, evening, night, and international calls of the customer
    
  - The total day, evening, night, and international charge of the customer
    
  - The total customer service calls of the customer
    
  - Whether or not the customer was 'true' or 'false' churn (true churn meaning that they have left the company, this will be the primary focus of the models)
  
  - The data appears to contain no missing values.

![Screen Shot 2021-09-14 at 12 59 03 PM](https://user-images.githubusercontent.com/66973223/133307580-1a80b896-69e0-421b-be42-56cf9b1a650e.png)

![Screen Shot 2021-09-14 at 12 59 26 PM](https://user-images.githubusercontent.com/66973223/133307730-af160cd2-91ee-44a7-8d75-c2f1f94f9436.png)

## Methods
* SyriaTel customer data will be used to create six different classification models to predict customer churn.

* The models will then be analyzed according to the precision metric.

* The best performing model will be analyzed for top feature importance.

* Business recommendations will then be presented. 

## Results & Conclusions

![Screen Shot 2021-09-14 at 1 43 50 PM](https://user-images.githubusercontent.com/66973223/133308192-1a07686d-bf1a-4521-acdd-ab94040dc43f.png)

The top performing model accorinding to the precision and ROC metrics was a Random Forest model using GridsearchCV in order to tune parameters. The top three features according to this model include:

1. Total Charge
2. Customer Service Calls
3. Total International Minutes

![Screen Shot 2021-09-14 at 1 43 24 PM](https://user-images.githubusercontent.com/66973223/133308059-17f13268-90d8-4dcc-8916-6924d859f7b6.png)

Based on the analysis, my main business recommendations are as follows:

1. Offer discounts/promotions to customers with higher than average total charge costs.

2. Offer discounts/promotions to customer who frequently call customer service. As well as improving customer service as a whole to better resolve issues. 

3. Create a competitive international plan to prevent international customers from leaving as well as attract more international customers overall.

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/jmg0144/churn-analysis-project/blob/main/SyriaTel-Customer-Churn-Analysis.ipynb) 

For additional information contact Justin Giovatto at justin.giovatto@gmail.com

## Repository Structure
├── data

├── README.md

├── SyriaTel-Churn-Analysis-Presentation.pdf

└── SyriaTel-Customer-Churn-Analysis.ipynb
