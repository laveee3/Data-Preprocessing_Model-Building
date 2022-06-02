# DataWrangling_ModelBuilding

Activity 1: Data Preparation and Preprocessing
----------------------------------------------
Here the customer is a power trading organization. We have just received a dataset from them and are trying to clean raw data in preparation for modeling. The data set includes hourly weather metrics as well as power output values in kWh.

Datasets:
Power_data_preprocessing.csv 
Weather_data_preprocessing.csv

Contraints:
1.	The customer has shared two datasets with inconsistent quality.
		a.	Some of the weather data is missing. Using the information in the column header, we determine the appropriate way to handle the missing data and explain the reasoning in the comments.
2.	The Power data is particularly useful for modeling purposes but needs some preprocessing.
	a.	Power usage can be affected by the day, month, or season. One of these timeframes will be chosen to create a categorical variable for it.
	b.	Will choose an appropriate scaling method. 
	c.	The company experienced a power outage due to high winds. On days where the wind was 30mph or above customers lost power. A filter will be created to remove the dates when customers lost power.


Activity 2: Model Building
---------------------------

An auto-insurance company is revamping its pricing model. The analyst developing the new price model believes that the best approach is to develop 2 models: one for customers who are likely to file an insurance claim within the first year of their contract and another one for all other customers. The analyst has prepared a clean dataset consisting of 10,000 customers and 10 engineered features which capture driving behavior. The data has already been preprocessed for you (i.e., no missing data, no outliers, data is scaled, no correlated features, and the classes are balanced).

The data is contained in claim_prediction.csv, where CLAIM = 1 means the customer filed a claim in the first year and CLAIM = 0 means the customer did not.

A model will be developed to predict if customers will file a claim in their first year based on their driving behavior.
