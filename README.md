# Amazon Customer Behavior analysis

## Table of contents

- [Project Overview](#Project-Overview)
- [Data Source](#Data-Source)
- [Tools](#Tools)
- [Data cleaning/Preparation](#Data-cleaning/Prepartion)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Analysis](#Data-Analysis)
- [Results/findings](#Results/findings)
- [Recommendations](#Recommendations)
- [Limitations](#Limitatios)
- [References](#References)
### Project Overview

This data analysis project aims to understand how customers interact with the platform,identify patterns in their browsing and purchasing behavior, uncover insights to optimize user experience and improve customer satisfaction

### Data Source

The primary dataset used for this analysis is the "Amazon Customer Behavior Survey.csv" file, containing information about survey answers by various customers

### Tools

- Excel - Data Cleaning
- SQL server - Data Analysis
- PowerBI - Creating visualization report


### Data Cleaning/Preparation

In the initial data preparation phase,we performedthe following tasks:
1. Data loading and inspection.
2. Handling Missing Values.
3. Data cleaning and formatting.

### Exploratory Data Analysis

EDA involved exploring the Survey data to answer questions, such as:

1.  what are customer preferences across product categories?
2.  how effective is Amazon's personalized recomendations?
3.  what are the factors influencing purchase decisions?
4.  what is the impact of reviews and ratings?
5.  how do customers discover products?
6.  how often do cusomers purchase products?
7.  what services do customrs appreciate the most ?
8.  how satisfied are customers after shopping ?
9.  what areas do amazon need to improve ?  

### Data Analysis

Include some interesting code/features worked with

```sql
SELECT purchase categories, COUNT(purchase categories) AS PC_Count FROM amazon
GROUP BY purchase categories
ORDER BY PC_Count DESC

SELECT product discovery source, COUNT(product disovery source) AS PDS_count
FROM amazon
Group BY product discovery source
ORDER BY PDS_Count DESC

SELECT service appreciation, COUNT(service apprecistion) AS SA_count
FROM amazon
GROUP BY service appreciation
ORDER BY SA_count DESC
```

### Results/findings

The analysis results are as follows:
- Beauty and Personal care and Clothing and Fashion are the most patronized categories by customers
- The product recommendation service provided by amazon is the most appreiated service by customers
- 33.72% of customers purchase products "few times a month"
- The average rating for the importance of customer rating is 2.48
- Top two factors affecting cart abandonment are customers "found a better price somewhere else" and customers "changed their mind"
- Most customers voted "customer service" as where amazon needs to improve
- 34.72% rated shopping satisfaction 3 out of 5 and that is the highest percentage
- 47.84% rated customer rating accuracy 3 out of 5 and that is the highest rating
- 39.37% answered "yes" to the question "do reviews help in making decisions"
- customers moderately rely on reviews to make purchasing decisions
- 45.35% answered "sometimes" to the question "is personalized recommendation helpful" which is the highest percentage
- 41.69% of customers do not get personalized reccomendations

### Recommendations

Based on the analysis, I recommend the following actions:
1. Improve the quality of customer service (take advantge of AI)
2. Invest in more beauty and personal care and clothing and fashion products
3. Ensure more customers get personalized reddomendations as it is the most appreciated service and almost half of the customers do not get personalized recommendations
4. Make the prices of products more competitve as that is the top major factor of cart abandonments

### Limitations

The dataset contained no identification values for customers so I could only conduct general analysis for this project

### References

1. ChatGPT


   
