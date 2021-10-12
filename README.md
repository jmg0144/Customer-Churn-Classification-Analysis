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
  
  - The data contains no missing values.

![Screen Shot 2021-10-12 at 5 29 28 PM](https://user-images.githubusercontent.com/66973223/137032113-ee4ab177-ea09-490a-88b2-75942a2c066e.png)

![Screen Shot 2021-10-12 at 5 30 06 PM](https://user-images.githubusercontent.com/66973223/137032197-4c16e344-a6ff-4009-b2af-c34d4b5820cc.png)

![Screen Shot 2021-10-12 at 5 30 19 PM](https://user-images.githubusercontent.com/66973223/137032241-f790f235-7eec-41bb-9699-4ff578dd0a82.png)

## Methods
* SyriaTel customer data will be used to create six different classification models to predict customer churn.

* The models will then be analyzed according to the precision metric.

* The best performing model will be analyzed for top feature importance.

* Business recommendations will then be presented. 

## Results & Conclusions
![Screen Shot 2021-10-12 at 7 35 40 PM](https://user-images.githubusercontent.com/66973223/137042873-202a3c36-4697-4bef-87eb-a32cafa073ef.png)

![Screen Shot 2021-10-12 at 7 15 41 PM](https://user-images.githubusercontent.com/66973223/137041678-44f948ea-d3fd-4d32-8c70-48added90f99.png)

![Screen Shot 2021-10-12 at 7 16 07 PM](https://user-images.githubusercontent.com/66973223/137041707-c80deb6d-5780-4066-b9f8-d3af2fa761b7.png)

![Screen Shot 2021-10-12 at 7 16 23 PM](https://user-images.githubusercontent.com/66973223/137041739-2c0f1955-42d0-4fc7-8028-11e0fd01781e.png)

![Screen Shot 2021-10-12 at 7 16 36 PM](https://user-images.githubusercontent.com/66973223/137041780-43fbd7f5-2831-4885-974e-93167d27bcff.png)

The top performing model accorinding to the precision and ROC metrics was a Random Forest model using GridsearchCV in order to tune parameters. The top three features according to this model include:

1. Total Charge
2. Customer Service Calls
3. Total International Minutes

![Screen Shot 2021-10-12 at 7 16 49 PM](https://user-images.githubusercontent.com/66973223/137041812-425271eb-9281-4e06-9d19-2e62df834887.png)

![Screen Shot 2021-10-12 at 7 17 46 PM](https://user-images.githubusercontent.com/66973223/137041827-57e86b29-be8a-4a6f-9746-57a5a61787d2.png)

![Screen Shot 2021-10-12 at 5 39 50 PM](https://user-images.githubusercontent.com/66973223/137032824-36860349-c232-4fac-acc2-35cd3932e7f4.png)

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
