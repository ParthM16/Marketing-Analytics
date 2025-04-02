# Marketing-Analytics
Marketing Analysis of Online Retail Business and campaign 

# Objective: 
### To propose strategies to the marketing manager to increase the conversion and average rating.</br>
Data: I've attached the .bak file</br>
Data Description:
  - Data from 2023 to 2025</br>
  - It contains customer details, customer reviews, product details, customer engagement data, and customer journey tables


# What I've Learnt
</br>

## 1. Data Cleaning in SQL Server



### **Product Table**
- Introduce a new `category` column based on the `Price` column.
- Categorize products into **Low**, **Medium**, and **High** price ranges.
- Query: </br>
<img src = "https://github.com/user-attachments/assets/e53268b2-aee6-4e3d-8f8d-29174a335331" width="700" height="350" ></br>

### **Customer Table**
- Enhance customer details by performing a join operation with the `Geography` table. </br>
Query: Run in Power BI during data load </br>
![image](https://github.com/user-attachments/assets/c10b9afd-f19a-4a8d-b8f6-122894ed8370)


### **Customer Engagement Table**
- Derive two new columns from a single source for better data segmentation.
- Standardize text columns to ensure consistency.</br>
Query: </br>
![image](https://github.com/user-attachments/assets/d616069d-eea1-4312-90e0-fb8f7e097499)


### **Customer Journey Table**
- Handle `NULL` values effectively.</br>
Query: </br>
![image](https://github.com/user-attachments/assets/cc0c0a22-031f-4a91-b8d5-de6da42ffb8c) </br>
![image](https://github.com/user-attachments/assets/70f1c9dc-445b-4f3e-88a9-c365a2c58ba4)


- Remove duplicate records to maintain data integrity.</br>
Query: </br>
![image](https://github.com/user-attachments/assets/3468c9b2-b99f-4ba6-84a5-a7b83313f0f5) </br>




### **Customer Review Table**
- Clean up text data using the `TRIM` function to remove unnecessary whitespace. </br>
Query: </br>
![image](https://github.com/user-attachments/assets/3023b1a5-7878-4d86-ad92-b8374b982538)



</br>
</br>


## 2. Sentiment Analysis using Python

### **Database Connection & Data Retrieval**
- Connects to an SQL Server database using `pyodbc` to fetch customer review data.

### **Sentiment Analysis**
- Utilizes **VADER** (Valence Aware Dictionary and Sentiment Reasoner) to compute a compound sentiment score for each review.
  - Sentiment score ranges from **-1** (most negative) to **+1** (most positive).

### **Sentiment Categorization**
- Combines the sentiment score with the customer rating to classify reviews into the following categories:
  - **Positive**
  - **Negative**
  - **Mixed Positive**
  - **Mixed Negative**
  - **Neutral**

### **Data Export**
- Saves the processed data, including sentiment scores and categories, to a CSV file for further analysis.

</br>
</br>

## 3. Data Visualization using Power BI

### **Data Modeling**
<img src="https://github.com/user-attachments/assets/252071d4-d10a-4d45-ab31-c678dfae440f" width="700" height="550" ></br>

### **Add Measures**
<img src = "https://github.com/user-attachments/assets/a5547bef-64a0-4cd0-9d0f-f587213feb84" width="300" height="350" ></br>

### **Dashboards**
<img src="https://github.com/user-attachments/assets/d3cebf75-1cea-4eb9-ad7b-608725a7b060" width="930" height="520" ></br>

<img src="https://github.com/user-attachments/assets/68eaa8b1-8fc5-4bec-8f65-5c47fc715ca2" width="930" height="520" ></br>

<img src="https://github.com/user-attachments/assets/2050d634-73e7-41a6-8f10-a478bdaad1fa" width="930" height="520" ></br>

<img src="https://github.com/user-attachments/assets/c720f883-1688-4b7f-a43f-6586e7dd4b28" width="930" height="520" ></br>



# Conclusion

- Enhanced marketing effectiveness for an online retailer by identifying the `top 3` product categories with `high conversion 
rates` but 32%-42% `non-positive` review sentiment across 3 years of data using `SQL` (data cleaning), `Python` (review sentiment analysis), and `Power BI` (built dashboard). </br>

- Presented `two data-driven` strategies:
  - A shift in content focus from blog (historically dominant) to video and social media 
  - A targeted campaign to convert non-positive reviews to positive ones for high-conversion products—to optimize marketing spending and improve product ratings.
 
Thank you @aliahmad-1987 for your guide and Please follow him on GitHub and LinkedIn!!


