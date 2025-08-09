# Black Friday Sales Data Analysis
Black Friday is a shopping holiday  that takes place on the day after Thanksgiving. It is known for its deep discounts and special deals on a wide range of products, including electronics, home goods, clothing, and more. Many retailers offer special doorbuster deals and extended hours on Black Friday, and it is traditionally one of the busiest shopping days of the year. 

This project explores the Black Friday Sales Data to uncover purchasing patterns and insights from various user demographics. The dataset includes multiple details about users, including their age, gender, occupation, and marital status, as well as information about the products they purchased during the Black Friday sale event. Through this project, we will walk through several steps to analyze the dataset, perform in-depth analysis of different columns, and combine multiple factors to gain actionable insights.

## Dataset Details
Dataset Name: Black Friday Sales Data
Dataset Size: 23 MB CSV file, containing over 537,000 rows and 12 columns.
Columns: User ID, Product ID, Gender, Age, Occupation, City Category, Stay in Current City Years, Marital Status, Product Categories, and Purchase amount.
Source: The dataset can be downloaded from here.
## Project Steps Overview:
### Walkthrough of the Dataset
#### Goal: Load the dataset, inspect its structure, and understand the contents.
#### Actions:
We begin by loading the Black Friday Sales dataset into a pandas DataFrame.
We examine the dataset’s structure and look for any missing values or discrepancies.
We perform a basic overview using df.info() to see the types of columns and the number of non-null entries.
Dataset link: Black Friday Sales Dataset
Analyzing Columns
Goal: Dive deeper into each column to understand their distributions and relevance.
Actions:
We focus on key columns like Gender, Age, Marital_Status, Product_Category, and Purchase.
We handle missing data by dropping columns that are too sparse, like Product_Category_2 and Product_Category_3.
We focus on understanding the unique values in various columns to gain an overview of the data. Specifically, we used unique() and nunique() functions to extract meaningful information from individual columns.
GitHub Link: Analyzing Columns Code
Analyzing Gender
Goal: Analyze the gender distribution of the customers and examine if there are any purchasing trends based on gender.
Actions:
Data Imbalance: A significantly higher number of male customers compared to female customers in the dataset.
Groupby Function: By using the groupby() function, we grouped the data by gender and found that male customers were responsible for a larger portion of the purchases.
GitHub Link: Analyzing Gender Code
Analyzing Age & Marital Status
Goal: Investigate how age groups and marital status affect purchasing behavior.
Actions:
We categorize users by age group and marital status, examining which groups tend to spend more during Black Friday sales.
GitHub Link: Analyzing Age & Marital Status Code
Multi Column Analysis
Goal: Combine multiple columns to analyze more complex relationships and derive insights from combinations of factors.
Actions:
We combine Age, Marital Status, and Gender to see if purchasing patterns vary when users' characteristics are combined.
By combining both factors with visualizations like pie charts and bar plots, we gained a clearer understanding of purchasing behavior across different age groups and marital statuses.
GitHub Link: Multi Column Analysis Code
Occupation and Products Analysis
Goal: Analyze how occupation influences purchasing behavior and which product categories are most popular among different occupations.
Actions:
We analyzed the Occupation, Product_ID, and Product_Category_1 columns. We aimed to understand the relationship between a customer’s occupation and the products they are most likely to purchase.
GitHub Link: Occupation & Products Analysis Code
Combining Gender & Marital Status
Goal: Further investigate the combined effects of gender and marital status on purchasing behavior.
Actions:
The final analysis combined Gender and Marital Status to examine if there was any significant relationship between these two factors and purchasing behavior.
We used Seaborn’s count plot to visualize how the combination of gender and marital status influences purchases. This allowed us to easily see which combinations were more likely to make purchases.
GitHub Link: Combining Gender & Marital Status Code
Conclusion
This project not only helps us understand the purchasing behavior of Black Friday shoppers but also provides insights into the influence of demographic factors like gender, age, marital status, and occupation on buying patterns. By using the Black Friday sales dataset, we walk through the process of cleaning the data, analyzing individual columns, and combining multiple features to uncover hidden patterns.
