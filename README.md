# Customer Segments Creation (usnupervised Learning)

## Project Overview


### Application Domain
The target market for this project are companies that collect vast amounts of data on customers, and want to understand the relationships hidden in their customer base. The knowledge extracted can assist the design of products and services that best satisfy the customers.


### Use Case
 - A wholesale distributor recently tested a change to their delivery method for some customers, by moving from a morning delivery service five days a week to a cheaper evening delivery service three days a week. 
 - Initial testing did not discover any significant unsatisfactory results, so they implemented the cheaper option for all customers. 
 - Almost immediately, the distributor began getting complaints about the delivery service change and customers were canceling deliveries, losing the distributor more money than what was being saved. 


### Goal

The the of the analysis is to find what types of customers are there, and which ones are sensitive to the delivery service proposed.
The premise is that unsupervised learning techniques can help to find out if similarities exist between customers, and how to best segment customers into categories that have different prorities.

### Process Outline

This is a summary of the steps proposed:  
1. subset a sample and determine if any product categories highly correlate with one another. 
2. preprocess the data by scaling each product category and then identifying (and removing) unwanted outliers. 
3. apply PCA transformations to the data
4. implement clustering algorithms to segment the transformed customer data. 
5. compare the segmentation found with an additional labeling
6. consider ways this information could assist the wholesale distributor with future service changes.


### Data analysis skills involved:

- feature scaling and outlier detection.
- interpreting data points that have been scaled, transformed, or reduced from PCA.
- analyzing PCA dimensions and construction of a new feature space.
- clustering a set of data to find hidden patterns.
- assessing information given by cluster data and application.



## Dataset
 
The data contains examples of clients of a wholesale distributor, and can be found in the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).

Note (m.u.) is shorthand for *monetary units*.

**Features**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 
2) `Milk`: annual spending (m.u.) on milk products (Continuous); 
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisnon - 1, Oporto - 2, or Other - 3} (Nominal) 


### Validation of results
The features `'Channel'` and `'Region'` will be held out in the unsupervised learning analysis — and they will be used at the end to validate the outcome of the segmentation process.


## Project Files

This project contains three files:

- `customer_segments.ipynb`: This is the main file where you will be performing your work on the project.
- `customers.csv`: The project dataset. You'll load this data in the notebook.
- `visuals.py`: This Python script provides supplementary visualizations for the project. Do not modify.
 


