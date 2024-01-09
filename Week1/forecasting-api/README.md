# FORECASTING API

To maximize the flow of goods, the company would like to help regional logistics planners get ahead
of particularly busy periods and to avoid product sell-outs. After discussions with
stakeholders and subject matter experts across the business, it is agreed that the ability
for planners to dynamically request and explore forecasts for particular warehouse items

## Data

This example will use the open Rossman stores dataset from Kaggle, which can be found
here: https://www.kaggle.com/pratyushakar/rossmann-store-sales

## Approach

We will use the following approach to create the anomaly detection service:

1. Standardize the data
2. Use DBScan Clustering algorithm to cluster the data
3. Identify the cluster with the most data points 
4. Identify the points not belonging to any of the major clusters as anomalies


