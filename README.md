
# [SQL] Explore Ecommerce Dataset
## I. Introduction
This project contains an eCommerce dataset that I will explore using SQL on [Google BigQuery](https://cloud.google.com/bigquery). The dataset is based on the Google Analytics public dataset and contains data from an eCommerce website.
## II. Business question
Customer Behavior doesn't describe who is shopping in your store, it describes how they shop there. It looks at factors like how often they shop, their product preferences, and how they feel about your marketing, sales, and service. Understanding these details helps businesses effectively communicate with customers. To understand customer behavior, we also need to classify customers into separate groups with the same behavioral tendencies or common characteristics (Customer Segmentation). For example, demographic classification based on age, gender, income, education level, and marital status; geographical classification based on continent, country, region, city, or town; or psychological classification based on personality, attitude, worldview, and interest.

Requirement: Apply customer transaction data to perform RFM analysis.
* Clearly present customer segments within the business and the performance of each segment.
* Provide appropriate suggestions for maintaining/developing/retaining/attracting each customer segment
## III. Dataset 
Dataset: adventureworks2019 (public Google BigQuery dataset)

Dataset Dictionary: [https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1](https://drive.google.com/file/d/1oYm32cdutBwHhkds4l-HznDYPZ5_WCxu/view)

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
<img width="631" alt="page 1" src="https://github.com/user-attachments/assets/85ba7812-859a-4b62-b696-99e5de2db99f">

### 2. Segment Dashboard
<img width="639" alt="page 2" src="https://github.com/user-attachments/assets/293de318-70fe-43b0-b151-05265a36e681">

### 3. Customer Dashboard
<img width="650" alt="page 3" src="https://github.com/user-attachments/assets/ef37ccb3-01f8-48a0-8fa3-88ed6b3cc87a">

## V. Insight
### Overview
#### Analysis of the Data
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
* Needing Attention (1.38%): The smallest group in both customers and revenue ($42,414), signaling low impact but potential for improvement with targeted actions.
##### Emerging Loyalty Segment:
* __Potential Loyalist__ (5.50%): Generates $162,402 from fewer customers, indicating the high potential to transition into higher-value segments
#### Recommendations
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
### Market 
* __North America__: Although customers in this market account for more than half of the total of customers (52%), its revenue for nearly three-quarters of total revenue (72%). This shows that customers in North America have larger card values ​​and average spending per customer than in other regions. In particular, the Champion segment in this region brings in the highest revenue, proving that this is a very important market to focus on retaining and developing.
* __Europe__: Customers in Europe account for a fairly high proportion (29%), but their revenue contribution is quite low (18%). For the Champion segment, revenue from Europe is much higher than that of other customer segments; revenue from other segments in the European market is very low.
* __Pacific__: This market accounts for 19% of total customers and contributes 10% of revenue. This is the region with the lowest average customer spending

