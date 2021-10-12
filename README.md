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
![Screen Shot 2021-10-12 at 5 30 39 PM](https://user-images.githubusercontent.com/66973223/137032333-4e222113-d04d-4fda-a342-f011bedc36fa.png)

![Screen Shot 2021-10-12 at 5 31 00 PM](https://user-images.githubusercontent.com/66973223/137032416-6a19d9e8-112d-41b7-8692-3587551ef698.png)

![Screen Shot 2021-10-12 at 5 31 18 PM](https://user-images.githubusercontent.com/66973223/137032461-74001738-2996-49b9-b833-f2d585399a2f.png)

![Screen Shot 2021-10-12 at 5 31 34 PM](https://user-images.githubusercontent.com/66973223/137032494-a78b7a03-a0ec-4969-a5f8-cc0935581607.png)

![Screen Shot 2021-10-12 at 5 43 24 PM](https://user-images.githubusercontent.com/66973223/137033232-e0492aec-690d-4bb9-bc42-75c448ff0bca.png)

The top performing model accorinding to the precision and ROC metrics was a Random Forest model using GridsearchCV in order to tune parameters. The top three features according to this model include:

1. Total Charge
2. Customer Service Calls
3. Total International Minutes

![Screen Shot 2021-10-12 at 5 43 11 PM](https://user-images.githubusercontent.com/66973223/137033276-6807f74b-f7c6-4902-9726-9932139151b6.png)

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
