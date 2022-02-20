# Predicting-Property-Maintenance-Fines

## Summary  
- Built a Random Forest Model with an auc over 75% to predict if a given blight ticket will be paid on time, to help the city of Detroit understand when and why a resident might fail to comply with a blight ticket. Provided the probability that the blight ticket will be paid on time for each entry.  
- Conducted data cleaning and data wrangling process of three datasets with over 250000 entries and 38 variables. Chose appropriate predictors for the prediction target.   

## Target

Every year, the city of Detroit issues millions of dollars in fines to residents and every year, many of these fines remain unpaid. To help the City of Detroit to solve one of the most pressing problems - blight violations, the first step is understanding when and why a resident might fail to comply with a blight ticket. Therefore, the target is using the given features to **predict if a given blight ticket will be paid on time**.

## Dataset
Source: [Detroit Open Data Portal](https://data.detroitmi.gov/)  
Two data files for use in training and validating your models: train.csv and test.csv. Each row in these two files corresponds to a single blight ticket, and includes information about when, why, and to whom each ticket was issued. The target variable is compliance, which is True if the ticket was paid early, on time, or within one month of the hearing date, False if the ticket was paid after the hearing date or not at all, and Null if the violator was found not responsible. Compliance, as well as a handful of other variables that will not be available at test-time, are only included in train.csv.  

## Conclusion

I built 3 classification models: Logistic regression, SVM, and random forest classification model. Finally I chose the random forest model with the highest auc that is over 75%, and output the probabilities that the ticket would be paid on time. 