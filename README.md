# Home_Sales

## Overview
The `Home_Sales.ipynb` file contained in the root directory is a Jupyter notebook intended to be run on Google Colab. It is intended to demonstrate some of the core tools used in handling Big Data files including the use of S3 storage buckets, the use of Spark to run SQL queries against CSV files, the use caching to improve performance, and the use of partitioning of data files in parquet format to improve performance.

The dataset consists of approximately 33,000 home sales including date of sale, date the home was built, price, number of bedrooms and bathrooms, square feet of living space, square feet of the lot, number of floors, whether or not the lot is "waterfront", and a "view" score from 0 to 100. 

Using Spark SQL, the data are analyzed to find average house prices by year built, average house prices year built, but filtered to certain sizes of houses, and average house prices by "view" rating. This last query is run on a temp table, on a cached temp table, and on a partitioned parquet temporary table to see performance differences with this particular dataset. 

All code is my own, but Xpert Learning Assistant was used to refresh my memory syntax for SQL rounding and group by functionality.

## Process
The initial library import is setup to be effective with the default VM's created by Google Colab, so the process is to open a new notebook in Google Colab, then import the `Home_Sales.ipynb` notebook and execute all cells. 
