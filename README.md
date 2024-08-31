# Power-BI-Project-Basket-Analysis

## Overview
This is a personal project focused on market analysis using Power BI. The project is inspired by a tutorial from [BI With Gurpreet](https://www.youtube.com/@biwithgurpreet). You can find the source video [here](https://www.youtube.com/watch?v=vK_njDjjP6I).

## About Dataset
The dataset, grocery.csv, was obtained from BI With Gurpreet and is originally sourced from Kaggle. It contains 7,835 rows of purchase orders from grocery stores. Each row represents a transaction/order and each column contains a grocery item. These orders are analyzed, and association rules are generated using Market Basket Analysis.

![image](https://github.com/user-attachments/assets/c4536a9a-adc3-4b57-a864-b3f1070a67ee)

## Market Basket Analysis 

Market Basket Analysis is a key technique used by large retailers to uncover associations between items. It identifies combinations of items that frequently occur together in transactions, helping retailers understand the relationships between the items that customers buy.

## Association Rule Mining
Association Rule Mining is used to analyze retail basket or transaction data. It aims to identify strong rules in transaction data using measures of interestingness, based on the concept of strong rules.

## Key Concepts
***Support*:** Indicates how popular an itemset is, measured by the proportion of transactions in which an itemset appears.

***Confidence*:** Indicates the likelihood of item Y being purchased when item X is purchased, expressed as {X -> Y}. It is measured by the proportion of transactions with item X in which item Y also appears.

***Lift*:** Indicates how likely item Y is purchased when item X is purchased, while controlling for how popular item Y is.

## Project Details
The project involves three key parts: data preparation, data visualization, and data analysis.

#### 1. Data preparation
Non-text values, such as backticks (`), were removed. Data was prepared by creating baskets of each two items and calculating support, confidence, and lift, as shown below.

![image](https://github.com/user-attachments/assets/2e1bacb7-6381-41f8-bbfb-d1cbab558139)

#### 2. Data Visualization
Four visualizations were prepared for the report:
1. **Donut Chart**: Displays the general spread of products. It helps in understanding which products are more popular among customers.
   
   ![image](https://github.com/user-attachments/assets/985098d6-c7a6-42dc-97d9-1860d7d0f7e4)

3. **Drill Down Network**: Highlights the sum of lift by baskets. It shows how often products are bought together, indicating the strength of association between items.
   
   ![image](https://github.com/user-attachments/assets/fd8ae5dd-a81a-4f21-9db7-2c4f656524ed)

5. **Matrix**: Provides detailed information, including the sum of support, sum of confidence for product pairs, and sum of lift for each basket. This helps in identifying strong product associations and their frequency.
   
   ![image](https://github.com/user-attachments/assets/fe2fa6ea-d77f-4758-9f4a-6ea6dcaba486)

7. **Scatter Graph**: Illustrates the relationship between the sum of lift and the sum of support for each basket. It helps in visualizing how often products are bought together and the strength of their association.
   
  ![image](https://github.com/user-attachments/assets/533e9259-f18d-4d46-bed7-9b2ce755780a)

## Results
**Most and Least Bought Items:** 
Whole milk is the most bought item, accounting for 5.81% of total items, while light bulbs are the least bought, making up 1%.

**Strongest Product Associations:**
*Root Vegetables and Herbs*: These have the highest sum of lift, with confidence levels of 6.03% and 40.94%, respectively. This indicates a strong association between these items, meaning customers frequently buy them together.
*Whipped/Sour Cream and Berries*: These items also show a strong association, with confidence levels of 11.58% and 25.88%, respectively. This suggests that customers tend to buy these items in pairs.

Drill Down Network shows that whole milk has the highest sum of lift at 92.47. This means that whole milk is frequently bought with other items, indicating its central role in shopping baskets.

## Conclusion

The data suggests that whole milk is a staple item in many shopping baskets, often bought with a variety of other products. The strong associations between root vegetables and herbs, as well as whipped/sour cream and berries, highlight common purchasing patterns. These insights can be used to optimize product placement, promotions, and inventory management.

