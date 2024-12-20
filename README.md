
# [PowerBI] RFM Segment Analysis
## I. Introduction
This project involves creating a comprehensive business intelligence dashboard for Adventure Works Cycles, a global bicycle manufacturer. The dashboard provides insight into customer segments based on the RFM model and suggestions for maintaining/developing/retaining/attracting each customer segment.
## II. Business question
Customer Behavior doesn't describe who is shopping in your store, it describes __how they shop__ there. It looks at factors like how often they shop, their product preferences, and how they feel about your marketing, sales, and service. Understanding these details helps businesses __effectively communicate__ with customers. To understand customer behavior, we also need to __classify__ customers into separate groups with the __same behavioral__ tendencies or __common characteristics__ (Customer Segmentation). For example, demographic classification based on age, gender, income, education level, and marital status; geographical classification based on continent, country, region, city, or town; or psychological classification based on personality, attitude, worldview, and interest.

Requirement: Apply customer transaction data to perform __RFM analysis__.
* Clearly present customer segments within the business and the performance of each segment.
* Provide appropriate suggestions for __maintaining/developing/retaining/attracting__ each customer segment
## III. Dataset 
Dataset: adventureworks2019 (public Google BigQuery dataset)

Dataset Dictionary: [here](https://drive.google.com/file/d/1oYm32cdutBwHhkds4l-HznDYPZ5_WCxu/view)

Dataset access:
* Log in to your Google Cloud Platform account and create a new project.
* Navigate to the BigQuery console and select your newly created project.
* In the navigation panel, select "Add Data" and then "Star a project by name".

Access BigQuery data from Power BI Desktop
* Launch Power BI and find the Get Data option in Home
* Search for the ODBC option from the data source list; select it, and click on Connect
* Select the DSN from the dropdown and click OK
* Connect BigQuery. The first time you connect to this DSN, you might need to enter the username, password and optional credential connection string properties and click Connect.
* Click Load to load all selected data from BigQuery.
## IV. Design Thinking Method
**Here are the five steps of design thinking:**
### Step 1 - Empathize
<img width="921" alt="st1" src="https://github.com/user-attachments/assets/35d617d6-2bc5-44fc-bfeb-9fe139bde68f">

### Step 2 -  Define point of view
<img width="920" alt="st2" src="https://github.com/user-attachments/assets/0dc7a56a-3102-4708-8afd-42041c9061fb">

### Step 3 - Ideate
<img width="920" alt="st3" src="https://github.com/user-attachments/assets/92d95080-2623-45f2-84dc-05680db34bed">

### Step 4 - Prototype and Review


## III. Visualization
### 1. Overview
<img width="793" alt="image" src="https://github.com/user-attachments/assets/135e4675-40db-4a5f-82a6-c0bcf74ffb35">

#### 1.1 Analysis of the Data
##### Revenue drivers:
* __Champions__: Despite accounting for only 10.81% of total customers, this segment generates the highest revenue, contributing $84,5M, demonstrating exceptional loyalty and high transaction values.
* __Can't Lose Them__ (11.20%): This segment contributed the second highest revenue at $18.5 million, showing they are still valuable even though these customers have not purchased again in a long time.
* __At Risk__ (9.64%): Generates a significant revenue of $8,6M, highlighting the need to retain these customers to avoid revenue loss.
* __Loyal Customers__ (9.49%): Because customers purchase so frequently, this segment contributes a considerable $7,316,328, underscoring its importance for long-term revenue stability.
##### Potential Growth Segments:
* __Promising__ (12.95%): Although this segment has high customer volume, the revenue contribution of $3,2M suggests there’s room for growth by increasing transaction frequency or value.
* __Recent Customers__ (17.02%): The largest segment by customer but contributes only $132,515. This is an important growth segment because they are new customers with recent transactions and a fairly high average spend.
##### Low-Engagement and Low-Revenue Segments
* __Hibernating__ (8.10%), __Lost__ (7.61%), and __About to Sleep__ (6.30%): They contribute minimal revenue. Their disengagement reflects a critical need for reactivation strategies.
* __Needing Attention__ (1.38%): The smallest group in both customers and revenue ($42,414), signaling low impact but potential for improvement with targeted actions.
##### Emerging Loyalty Segment:
* __Potential Loyalist__ (5.50%): Generates $162,402 from fewer customers, indicating the high potential to transition into higher-value segments
#### 1.2 Recommendations
#####  Focus on High-Revenue Segments (Champions, Can't Lose Them, At Risk, Loyal Customers)
* __Champions__: Maintain loyalty through personalized rewards, exclusive benefits, and early access to products/services.
* __Can't Lose Them__: Reactivate engagement with high-value offers or personalized campaigns addressing their preferences; collect their feedback to improve and prevent them from moving to lower value segments.
* __At Risk__: Prioritize this group with retention campaigns, such as discounts or bundled offers; conduct surveys to identify their concerns and address them effectively
* __Loyal Customers__: Encourage upselling by suggesting complementary products; enhance loyalty program
##### Grow Emerging Segments (Promising, Recent Customers, Potential Loyalist):
* __Recent Customers__: Personalize offers to encourage repeat purchases.
* __Promising__ and __Potential Loyalist__: Provide targeted promotions or loyalty rewards to increase transaction frequency and elevate them to higher-value segments
##### Revive Low-Engagement Segments (Hibernating, Lost, About to Sleep, Needing Attention)
* __Hibernating__ and __Lost__: Design customer attraction campaigns with attractive offers
* __About to Sleep,  Needing Attention__: Use limited-time offers to reignite interest

### 2. Segment Dashboard
<img width="792" alt="image" src="https://github.com/user-attachments/assets/60e88efd-f3f8-4247-8629-9a5a17a08a4b">

In this dashboard, we will analyze according to 2 views of the segment: market and purchase method

#### 2.1 Market 
##### 2.1.1 Analysis of the Data
* __North America__: Although customers in this market account for more than half of the total of customers (52%), its revenue for nearly three-quarters of total revenue (72%). This shows that customers in North America have larger card values ​​and average spending per customer than in other regions. In particular, the __Champion__ segment in this region brings in the highest revenue, proving that this is a very important market to focus on retaining and developing.
* __Europe__: Customers in Europe account for a fairly high proportion (29%), but their revenue contribution is quite low (18%). For the __Champion__ segment, revenue from Europe is much higher than that of other customer segments; revenue from other segments in the European market is very low.
* __Pacific__: This market accounts for 19% of total customers and contributes 10% of revenue. This is the region with the lowest average customer spending
##### 2.1.2 Recommendations
* __North America__: Focus on retaining and expanding the high-value Champion segment
* __Europe__: Increase revenue from non-Champion segments with targeted engagement and promotions
* __Pacific__:Encourage higher spending with bundled offers and discounts
#### 2.2 Purchase method 
##### 2.2.1 Analysis of the Data
* Although online orders account for an overwhelming majority (88%), online revenue only accounts for 74%. Offline orders account for a small percentage (12%) but contribute to 26% of total revenue. This shows that the average card value of online orders is lower than offline orders.
* __Champion__'s offline order volume is very high (3017), indicating that __Champion__ customers tend to shop more through offline channels. Their online orders (4014) are comparable to other segments such as __Loyal__ and __At-Risk__, indicating that offline orders are the main factor driving the total number of orders in the __Champion__ segment.
##### 2.2.2 Recommendations
* __Online__: Encourage online shopping, convenient delivery service.
* __Offline__: Special promotions, improve in-store experience
  
### 3. Customer Dashboard
<img width="792" alt="image" src="https://github.com/user-attachments/assets/30cd8169-bd17-40f7-8244-d50fd3166b49">

Through this dashboard, users can look up specific information of each customer.

## V. Conclusion






