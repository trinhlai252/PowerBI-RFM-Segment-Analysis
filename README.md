# PowerBI-RFM-Segment-Analysis
Utilized Power BI to analysis RFM segment
# PBI_RFM_ANALYSIS

## I. Introduction
### 1. Business question
<p>Sales representatives from regional sales offices have assigned sales territories in the United States, Canada, England, Australia, Germany, and France. Each regional office consists of several sales representatives and a team manager. In their daily sales activities, sales representatives use both laptops and Handheld PCs that run Microsoft® Windows CE. A typical work day for a sales representative starts with the representative dialing in to the regional office and downloading current data such as inventory, product, and promotional information. During customer visits, the sales representative takes orders on the laptop or Handheld PC. At the end of each day, the sales representative sets up appointments for the following day or week, checks the appointments of other representatives in the area for possible collaboration, and updates the contact list. The sales representative dials back into the regional office, sends updated information, and receives any new internal communications from the base office or regional office. The company currently uses Microsoft Outlook® for email.</p>
<p>The sales teams have identified the following requirements that will enable them to perform their jobs better:</p>
<p>Customer segmentation and profiling:</p>
<ul>
  <li>Analyze customers based on their purchase behaviours: RFM (recency, frequency, and monetary value of a transaction)</li>
  <li>Who are the best customer across all product lines? With whom should the sales team focus its efforts for building long-term relationships?</li>
  <li>What products are popular and at what rate among customer group?</li>
</ul>

### 2. Dataset

<p>Dataset: adventureworks2019 (public Google BigQuery dataset)</p>
<p>Dataset dictionary: Please reach file "Data Dictionary" attached above</p>
<p></p>Dataset Schema:  https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1</p>
<p>Dataset access:
  <ul>
  <li>Log in to your Google Cloud Platform account and create a new project.</li>
  <li>Navigate to the BigQuery console and select your newly created project.</li>
  <li>In the navigation panel, select "Add Data" and then "Star a project by name".</li>
  <liEnter the project name "adventurework2019"></li>
</ul>

## II. Apply design-thinking mindset
### 1. Empathize
<img width="1200" alt="emphathy" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/0efe5635-06f2-496a-93c4-83aaf6c2d092">

### 2. Define point of view
<img width="1200" alt="stage2" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/e844c392-3adf-4181-b3e4-377346051270">

### 3.Ideate
<img width="1200" alt="stage3" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/4eb68089-75c3-4114-b5c6-d749337b61b1">

### 4. Prototype and Review
<img width="1200" alt="stage 4" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/d15ddc7c-99e8-44c7-b5c1-81a6d37bbdec">

## III. Main Process
### 1. Connect data to PBI and modeling
<img width="1200" alt="Screenshot_8" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/e808fd91-5403-45df-aa7c-abe09f984460">

### 2. Build Dashboard
<p><b>Sale Overview</b></p>
<img width="1200" alt="Screenshot_9" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/d58ccddc-82ee-4665-943d-d28881fd7ee3">
<p><b>Customer</b></p>
<img width="1200" alt="Screenshot_10" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/2686126a-7861-4975-9ad7-7ef6c1aa1201">
<p><b>Product</b></p>
<img width="1200" alt="Screenshot_12" src="https://github.com/TAQUOCANH/PBI_RFM_ANALYSIS/assets/135592751/c89e75b8-3a12-4525-8c42-4c053f3dd162">

<h2>IV. Insights</h2>

<h3>Market Focus</h3>
<ul>
    <li><strong>Primary Markets:</strong> The United States, Canada, and Australia contribute 80% of the revenue.</li>
    <li><strong>Profit Focus:</strong> The United States and Australia generate 60% of the profit.</li>
</ul>

<h3>Customer Segmentation and Market Insights</h3>
<h4>US Market</h4>
<ul>
    <li><strong>Customer Base:</strong>
        <ul>
            <li>Online customers: 95% of the customer base, contributing only 15% of the revenue.</li>
            <li>In-store customers: 85% of the revenue.</li>
        </ul>
    </li>
    <li><strong>Key Customer Segments:</strong>
        <ul>
            <li>Largest customer groups: "New Customer," "Promising," and "Cannot Lose Them."</li>
            <li>High revenue and profit groups: "Promising," "Cannot Lose Them," "At Risk," "Loyal," and "Champions."</li>
        </ul>
    </li>
    <li><strong>Revenue Contribution:</strong>
        <ul>
            <li>B2B: "Cannot Lose Them" and "Champions" contribute over 80% of revenue but with low or negative profit.</li>
            <li>B2C: "Promising," "At Risk," and "Loyal" groups generate over 95% of revenue and profit.</li>
        </ul>
    </li>
</ul>

<h4>AU Market</h4>
<ul>
    <li><strong>Customer Base:</strong>
        <ul>
            <li>Online customers: 99% of the customer base, generating 85% of revenue.</li>
        </ul>
    </li>
    <li><strong>Key Customer Segments:</strong>
        <ul>
            <li>Largest customer groups: "At Risk," "Champions," and "Loyal."</li>
            <li>High revenue and profit groups: "At Risk," "Champions," and "Loyal."</li>
        </ul>
    </li>
    <li><strong>Market Type:</strong> Primarily B2C.</li>
</ul>

<h3>Product Insights</h3>
<h4>US Market</h4>
<ul>
    <li><strong>"Promising" Segment:</strong>
        <ul>
            <li>Highest total profit from Road Bikes ($465.92K), followed by Mountain Bikes ($289.23K) and Touring Bikes ($123.56K).</li>
        </ul>
    </li>
    <li><strong>Focus Products:</strong> Road Bikes and Mountain Bikes.</li>
</ul>

<h4>AU Market</h4>
<ul>
    <li><strong>"Champions" Segment:</strong>
        <ul>
            <li>Highest profit from Road Bikes ($660.1K), followed by Mountain Bikes ($497.45K).</li>
        </ul>
    </li>
</ul>

<h2>V. Recommendations</h2>

<h3>Market Strategy</h3>
<ul>
    <li>Focus efforts on the United States and Australia to maximize revenue and profit.</li>
</ul>

<h3>Customer Strategy</h3>
<h4>US Market</h4>
<ul>
    <li><strong>Promising Segment:</strong>
        <ul>
            <li>Prioritize for long-term growth.</li>
            <li>Engage with special experiences and advertisements.</li>
        </ul>
    </li>
    <li><strong>B2B Segments:</strong>
        <ul>
            <li>Offer new products with special offers to "Champions" and "Cannot Lose Them" groups to increase product awareness.</li>
        </ul>
    </li>
    <li><strong>Overall:</strong> Build long-term relationships with the "Promising" customer segment.</li>
</ul>

<h4>AU Market</h4>
<ul>
    <li><strong>Champions Segment:</strong>
        <ul>
            <li>Focus for long-term benefits.</li>
            <li>Enhance after-sales services and provide special offers to increase customer loyalty.</li>
        </ul>
    </li>
</ul>

<h3>Product Strategy</h3>
<h4>US Market</h4>
<ul>
    <li><strong>Promising Segment:</strong>
        <ul>
            <li>Invest in promoting Road Bikes and Mountain Bikes.</li>
        </ul>
    </li>
    <li><strong>Overall:</strong>
        <ul>
            <li>Tailor product offerings to meet the preferences of high-profit segments.</li>
        </ul>
    </li>
</ul>

<h4>AU Market</h4>
<ul>
    <li><strong>Champions Segment:</strong>
        <ul>
            <li>Prioritize Road Bikes and Mountain Bikes.</li>
        </ul>
    </li>
    <li><strong>Overall:</strong>
        <ul>
            <li>Ensure high-quality and competitively priced products to maintain profitability.</li>
        </ul>
    </li>
</ul>
