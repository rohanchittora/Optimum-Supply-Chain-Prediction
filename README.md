# Optimum-Supply-Chain-Prediction
Predict optimum supply of a product to the warehouses to ensure optimum demand supply match to prevent inventory loss

# 1. Business Problem¶
## 1.1 Description
An FMCG company entered into the instant noodles business two years back. Their higher management has noticed that there is a miss match in the demand and supply. Where the demand is high, supply is pretty low and where the demand is low, supply is pretty high. In both ways, it is an inventory cost loss to the company.
## 1.2 Problem Statement
Since there is a demand supply mismatch, it leads to inventory loss to the company. Therefore company wants to optimize the supply quantity in every warehouse in the entire country.
## 1.3 Source/Link of Dataset
https://drive.google.com/drive/folders/10zVYtUH-74K7nvXIGu3XZnrsSF44k9Jm
## 1.4 Real-world/Business objectives and constraints.
- Analyze the demand pattern in different pockets of the country
- Interpretability is important
- Minimize errors as these can lead to inventory loss
# 2. Machine Learning Problem Formulation
## 2.1 Data
## 2.1.1 Data Overview
Source: https://drive.google.com/drive/folders/10zVYtUH-74K7nvXIGu3XZnrsSF44k9Jm

We have one file named Dataset.csv which contains the data/information about the nature of the location and inventory management.
Number of columns in dataset: 24
Number of rows in dataset: 25000
Data dictionary has been given with the above source link
## 2.1.2 Example Data Point
Ware_house_ID,WH_Manager_ID,Location_type,WH_capacity_size,zone,WH_regional_zone,num_refill_req_l3m,transport_issue_l1y,Competitor_in_mkt,retail_shop_num,wh_owner_type,distributor_num,flood_impacted,flood_proof,electric_supply,dist_from_hub,workers_num,wh_est_year,storage_issue_reported_l3m,temp_reg_mach,approved_wh_govt_certificate,wh_breakdown_l3m,govt_check_l3m,product_wg_ton

WH_100000,EID_50000,Urban,Small,West,Zone 6,3,1,2,4651,Rented,24,0,1,1,91,29,,13,0,A,5,15,17115

WH_100001,EID_50001,Rural,Large,North,Zone 5,0,0,4,6217,Company Owned,47,0,0,1,210,31,,4,0,A,3,17,5074

## 2.2 Mapping to real-world problem to an ML problem
## 2.2.1 Type of Machine Learning Problem
We have to predict the weight(in tonnes) to be supplied ==> Regression Problem

## 2.2.2 Performance Metric
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R-Squared
