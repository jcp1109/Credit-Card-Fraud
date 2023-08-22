# Credit Card Data Fraud Detection

**Jean Pacheco**  
*University of Central Florida*  
*Machine Learning*  

## Abstract

Credit card fraud is a pervasive challenge in the financial world, necessitating effective preventive measures. This project employs machine learning techniques to aid financial institutions in mitigating fraudulent activities. The project utilizes a comprehensive database of credit card transactions, encompassing various transaction aspects. It predicts that certain factors, such as age, play a pivotal role in determining vulnerability to fraud. By training classification and regression models on preprocessed data, the project identifies key variables correlated with fraudulent transactions. The study suggests implementing stricter verification processes, focusing on transaction timestamps, to curb fraud occurrences.

## Introduction

Credit card fraud is a ubiquitous threat affecting individuals across socioeconomic strata. In 2021 alone, there were approximately 389,737 reported cases of credit card fraud, resulting in a staggering $32.34 billion in losses (E. Ortiz, 2021). Financial institutions must prioritize fraud prevention to ensure customer trust and security. This research project aims to analyze a dataset of genuine and fraudulent credit card transactions to identify indicators of fraudulent activities. By scrutinizing variables like cardholder information, transaction location, and more, the research seeks to unveil patterns underlying credit card fraud.

## Important Definitions and Problem Statement

The research utilizes a dataset containing credit card transaction indicators, encompassing credit card information, personal details, transaction timestamps, locations, merchant information, and transaction categories. The research endeavors to identify the indicators most indicative of credit card fraud. However, challenges arise due to uncertainties surrounding the security of credit card processors and the authenticity of card numbers in the dataset.

## Overview of Proposed Approaches/Systems

The research employs a machine learning pipeline consisting of problem identification, data analysis, data preprocessing, modeling, and visualization. It focuses on binary classification and regression tasks to predict the fraudulence of transactions. The pipeline involves data separation, transformation of variables like 'age' and 'transaction timestamp,' and identification of relevant indicators correlating with the target variable 'is_fraud.'

## Technical Details of Proposed Approaches/Systems

The research initially separates training and test datasets and identifies the target variable 'is_fraud.' It transforms the 'age' variable into a derived 'age' variable by comparing birthdates with the current date. It also extracts 'weekday' and 'hour' from the 'trans_date_trans_time' variable to examine correlations between transaction timing and fraudulence.

Key indicators demonstrating correlation with 'is_fraud' are 'gender,' 'age,' 'weekday,' 'state,' 'hour,' and 'category.' The analysis reveals insights such as higher fraud likelihood among male cardholders, increased risk for individuals above 65 years old, and concentrated fraudulent activities in specific states. Fraudulent transactions are more common on Fridays and during later hours.

## Experiments

Through systematic elimination of insignificant variables, the research employs machine learning algorithms (e.g., Logistic Regression, Random Forest) on the test dataset. The Random Forest algorithm achieves a high accuracy score of 99.79%, demonstrating its effectiveness in fraud detection.

## Conclusion

Credit card fraud demands serious attention from financial institutions to maintain customer trust and security. This research sheds light on transaction timings and preventive measures, such as multi-factor authentication, to combat fraud effectively.

## References

- E. Ortiz, "Credit Card Fraud Statistics," Bankrate, 06-Jul-2021. [Online]. Available: https://www.bankrate.com/finance/credit-cards/credit-card-fraud-statistics/#fraud
- Data retrieval: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
- Code: https://github.com/jcp1109/Credit-Card-Fraud/blob/main/Credit_Card_Fraud.ipynb

## Illustrations

*Figures 1-8: Refer to the original document for visualizations.*
