# BATCH ANOMALY DETECTION SERVICE

To create an anomaly detection service to find rides that have unusual ride time or ride length behaviour.

## Data

The data is a subset of the [NYC Taxi and Limousine Commission](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page) data. The data is stored in a public S3 bucket.

It contains the following fields:
* ride time
* ride length
* ride speed

## Approach

We will use the following approach to create the anomaly detection service:

1. Standardize the data
2. Use DBScan Clustering algorithm to cluster the data
3. Identify the cluster with the most data points 
4. Identify the points not belonging to any of the major clusters as anomalies


