Walmart E-Commerce Analysis: Customer Segmentation & Product Recommendation

Walmart is a multinational retail corporation based in the United States. It operates a chain of hypermarkets, discount department stores, and grocery stores.

-  Since 2019, Walmart's e-commerce sales have grown by over 70%
-  The company collects over 2.5 petabytes of data every hour
-  As of 2013, its e-commerce platform generates over $100 billion annually from online sales

DATASET OVERVIEW

The dataset includes key customer and transaction features:
  - Gender
   - Age
   - Occupation
   - City_Category
   - Stay_In_Current_City_Wars
   - Marital_Status
   - Product_Category
   - Purchase

MACHINE LEARNING MODEL

We developed two machine learning models:
1. CUSTOMER SEGMENTATION
   
For customer segmentation, we applied the K-Means algorithm, an unsupervised learning method.
- Why K-Means? It automatically groups customers into clusters based on behavioral and demographic similarities, without labeled data.
- Preprocessing:
  - Categorical variables (Gender, Age, City_Category, etc.) were converted using One-Hot Enconding to ensure each categroy was treated independently, which is essential for distance-based algorithms like K-Means
  - We used the elbow for distance-based algorithms like K-Means
2. PRODUCT RECOMMENDATION

For product recommendation, we used a K-Neares Neighbors (KNN) classification model
- Objective: Recommend the most likely product category to each user based on their demographic and behavioral data
- Why KNN?
  - It is a simple, intuitive, and effective algorithm that compares new users to similar past users
  - It calculates the distance between feature values to identify the most similar users and predict their likely product preferences
- Preprocessing:
  - Label Encoding was used for binary variables likes Gender
  - One-Hot Encoding was applied to variables like Age and City_Category to avoid implying any ordinal relationship

KEY INSIGHTS

ANALYSIS BY GENDER
- Male users account for -75% of total purchase volume
- Recommendation: Increase female participation through personalized marketing exclusive benefits, and targeted promtions

ANALYSIS BY AGE GROUP
- The 26-35 segment is the top spender, with over $2 billion in purchase
- 18-25 and 36-45 also show strong engagement
- Recommendation: Focus on lifestyle, tech, and household product campaigns. Leverage digital and social media to target younger audiences

KNN PREDICTION MODEL

Objective: Predict product categories based on user features
Model Accuracy: -78%
Evaluation: A confusion matrix and classification report were used to asses the model's performance

CONCLUSION

The ability to accurately segment customers and predict their product preferences enables more personalized user experiences and increse the likelihood of conversions. These insights can drive strategic marketing, optimize product targeting, and ultimately boost e-commerce sales for Walmart
