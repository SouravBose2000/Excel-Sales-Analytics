*******************
# **Sales Report**
*******************

### **Project Overview**

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using Excel in their company to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms of all the aspects like sales and finance.

I worked on this project by following the Codebasics Excel Course, Link to the course is [here](https://codebasics.io/courses/excel-mother-of-business-intelligence).

you can find the full report file here :
    
- 📄 [View Report (PDF)](https://github.com/SouravBose2000/Excel-Sales-Analytics/tree/main/Project/PDF)

- 📊 [View Report (Excel)](https://github.com/SouravBose2000/Excel-Sales-Analytics/tree/main/Project/Excel)

*******************
### **Technical & Soft Skills:**
- Proficiency in ETL methodology (Extract, Transform, Load).
- Skills to generate a date table using Power Query.
- Ability to derive fiscal months and quarters.
- Establishing data model relationships with Power Pivot.
- Applied data modeling techniques such as the star schema to structure relationships between tables efficiently.
- Proficiency in incorporating supplementary data into an existing data model.
- Utilizing DAX to create calculated columns.
- Used Power Query for cleaning, shaping, and transforming data efficiently within Excel.
- Applied DAX language to create calculated columns, measures, and KPIs for data analysis.
- Used Power Query M language to write advanced data transformation logic beyond the UI.
- Used Pivot Tables to create dynamic summaries and insights using Excel’s Pivot Table features.
- Applied Conditional Formatting to visually highlight patterns, trends and variances.
- Used Macros/VBA to Automate repetitive Excel tasks using recorded macros and VBA scripting.
- Used the DIVIDE function to prevent division-by-zero errors.
- And more 😅

### **Soft Skills:**

- What are all the questions should be asked before staring the project.
- Refined understanding of Sales & Finance Reports.
- Designing user-centric reports with empathy in mind.
- Optimization of report generation through meticulous fine-tuning.
- Developing a systematic approach to devising a report building plan.

*******************
### **GitHub** 

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

*******************
### **Business Related Terms Learned**

- Gross Price
- Net Invoice Sale
- Post Discount
- Net Sales
- COGS – Cost of Goods Sold
- Gross Margin
- Target
- Fiscal Year
- YTD – Year to Date
- YTG – Year to Go
- Customer
- Consumer
- Brick & Mortar
- E-Commerce
- Direct
- Retailer
- Distributor

*******************
### **Company’s back ground**

AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel.

- Retailers
- Direct
- Distributors

*******************

### **Dataset Understanding**

AltiQ hardware required some reports on sales analytics and finance analytics, so they given analytics team some requirement files. Now, this requirement file is given by Atliq business users to data analytics team. Now analytics team have to build reports using these requirement files. Those requirement files contains some sales CSV files, let’s explore them.

**Dimension table :** These tables contain static or descriptive data such as details about customers, products, or markets. We have the following dimension tables: dim_customer, dim_market, dim_product.

- **dim_customer**
     - **189** distinct customer code
     - **67** distinct and **17** unique customers thorough out the market
     - **23** distinct markets (ex India, USA, spain)
     - **2** types of platforms
          - Brick & Motors - Physical/offline store
          - E-commerce - Online Store (Amazon, flipkart)
     - **3** channels
          - Retailer
          - Direct
          - Distributors

&nbsp;

- **dim_market**
     - **23** distinct markets (ex India, USA, spain)
     - **6** distinct and **1** unique sub-zones
     - **3** regions
          - APAC
          - EU
          - nan

&nbsp;

- **dim_product**
     - **298** distinct Product code 
     - **3** distinct Divisions and **6** distinct Segments
          - P & A
            - Peripherals
            - Accessories
          - PC
            - Notebook
            - Desktop
          - N & S
             - Networking
             - Storage
        - There are **13** distinct categories, Like Internal HDD, keyboard
        - There are different variants available for the same product

**Fact table :** These tables store transactional or measurable data. We have the following fact tables: fact_sales_monthly, ns_targets_2021, fact_sales_monthly_with_cost.

**fact_sales_monthly**- This fact table contains monthly transactional-level data on product sales and associated costs, including quantity sold, net sales, freight charges, and manufacturing expenses.

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| date              | This column has the monthly sales data from September 2018 to August 2021                               |
| product_code      | This column is a unique identifier for each product sold, has repeated values because the same product is part of many sales transactions           |
| customer_code     | This column is a unique identifier for each customer, reflects purchases made by the same customer across different periods                                                 |
| Qty              | This column indicates the quantity of units sold per product in each transaction                                           |
| net_sales_amount  | This column captures total net revenue generated from each transaction  

&nbsp;

**ns_targets_2021**
        - This fact table contains the monthly net sales targets for different markets (countries), covering the period from 1st September 2020 to 1st August 2021.

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| date              | This column Represents the month and year for each sales target entry, ranging from September 2020 to August 2021 |
| market      | This column indicates the country or regional market for which the sales target is set, Contains **23** distinct markets (e.g., India, USA, Spain) |
| ns_target     | This column indicates the monthly net sales target amount for each market |

&nbsp;

**fact_sales_monthly_with_cost**
        - This table is an extended version of fact_sales_monthly. It includes the same columns — date, product_code, customer_code, Qty, and net_sales_amount — with two additional columns: freight_cost and manufacturing_cost. It contains monthly transactional-level sales data enriched with cost-related details.

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| freight_cost              | This column has details of shipping, delivery and other cost associated with each transaction |
| manufacturing_cost      | This column shows the cost of producing the product sold in each transaction |

*******************
### **Planning Before Report Building**

Before jumping into building the final reports, it’s important to follow a structured, step-by-step approach. This ensures clarity, reusability, and a scalable reporting structure. In this project, we planned to build reports for Sales analytics and finance analytics.

#### **Sales Report :**

- **Project objective:**

   **1.** Create a _[customer performance report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Customer%20Performance%20Report.pdf)_ 

   **2.** Conduct a comprehensive comparison between _[market performance and sales targets](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Market%20Performance%20vs%20Target%20Report.pdf)_

- **Purpose of sales analytics:** Empower businesses to monitor and evaluate their sales activities and performance.

- **Importance of analyzing sales data:** Identify sales patterns and track key performance indicators (KPIs).

- **Role of reports:** Determine effective customer discounts, facilitate negotiations with consumers, and identify potential business expansion opportunities in promising countries.

&nbsp;
#### **Finance Report :**

- **Project objective:** 

    **1.** Create Profit and Loss (P&L) reports by _[Fiscal Year](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/P%26L%20Statement%20by%20Fiscal%20Year.pdf)_ & _[Months](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/P%26L%20Statement%20by%20Months.pdf)_ 

   **2.** Create Profit and Loss (P&L) reports by _[Markets](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/P%26L%20Statement%20by%20Markets.pdf)_

- **Purpose of sales analytics:** Evaluation of financial performance, support decision-making, and facilitate communication with stakeholders.

- **Importance of analyzing Finance data:** Aid in benchmarking against industry peers and previous periods Foundation for budgeting and forecasting.

- **Role of reports:** Align financial planning with strategic goals Instill confidence in the organization's financial outlook.

There are other reports like _[Product Based Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Product%20Based%20Report.pdf)_, _[Division Level Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Division%20Level%20Report.pdf)_, _[Top and bottom products - QTY Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Top%20and%20bottom%20products%20-%20QTY%20Report.pdf)_, _[New products - 2021 Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/New%20Products%20-%202021%20Report.pdf)_, _[Top 5 countries Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/Top%205%20countries%20Report.pdf)_ and _[GM% (sub_zone) Report](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Project/PDF/GM%20%25%20by%20Subzone%20Report.pdf)_.
        
To prepare for these, we followed these steps:
- **ETL Process – Extract, Transform, Load :**
The Atliq business team provided the analytics team with requirement files containing raw sales data in .csv format. These files include monthly transactional data from Atliq Hardware’s sales operations.We first imported the CSV files into Excel, which is known as the **Extract** step — this brings the raw data into our environment for further processing. Next, we used Power Query to clean, filter, rename columns, remove nulls, and apply business logic as needed — this is the **Transform** step, where we shape the data into a usable form. Finally, the transformed data was loaded back into Excel across structured sheets, ready for modeling and analysis in Power Pivot — this is the **Load** step.
- **Identify Report Components**
        - We first listed all the required components (fields/measures) needed for both reports. This helped us map which fields come from which table (e.g., sales data from the fact table, customer details from the dimension table).
- **Create dim_date Table**
        - The dataset didn’t include a dedicated date dimension, so we created a dim_date table using Power Query. This date table allows for advanced time intelligence functions such as Year-to-Date (YTD), Month-over-Month (MoM), and more.
- **Build the Data Model**
        - Data modeling plays a vital role and is considered as the basement of report.
        - Poor data modeling affects the over all performance of the report.
        - In this project, we have followed Snowfall data modeling method.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Data_Model.png" class="center">

*******************
### **Report designing**

Based on the mockup files received as requirement, the team will start designing the report and create measure as and when required

#### **Customer Performance Report**

In customer performance report highlights the net sales for individual customer for 2019 and 2020 and 2021, It allows for a year-over-year comparison to evaluate customer performance. The report also highlights the year-over-year percentage growth in net sales from 2020 to 2021.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Customer%20Performance%20Report.png" class="center">

#### **Market Performance VS Target Report**

The Market Performance Report provides a breakdown of net sales by market (country) for each individual year, allowing stakeholders to analyze how different countries have performed over time. This report includes 2021 sales targets and compares them against the actual net sales for 2021, highlighting the gap between target and performance.This report also displays the percentage variance from the target using conditional formatting, enabling quick identification of underperforming or outperforming markets.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Market%20Performance%20vs%20Target%20Report.png" class="center">

#### **P & L by Fiscal Years Report**

The Profit & Loss (P & L) by Fiscal Years Report summarizes key financial metrics — including Net Sales, COGS (Cost of Goods Sold), Gross Margin, and Gross Margin Percentage — across the fiscal years 2019, 2020, and 2021. In addition, this report also shows a comparison column (21 vs 20), which highlights the percentage change from 2020 to 2021 for each metric. This provides a quick view of year-over-year performance improvements or declines. Interactive filters for customer, market, division, and region allow users to slice the data and view financial performance from multiple perspectives.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/P%26L%20Statement%20by%20Fiscal%20Year.png" class="center">

#### **P & L by Fiscal Months Report**

The Profit & Loss (P & L) by Fiscal Months Report presents monthly financial performance data across the fiscal years 2019, 2020, and 2021. The report breaks down key metrics such as Net Sales, COGS (Cost of Goods Sold), Gross Margin, Gross Margin % , These metrics are displayed month-by-month and grouped into fiscal quarters (Q1–Q4), helping users analyze seasonal patterns and monthly business performance. The bottom section of the report includes Net Sales comparison metrics, specifically 2021 vs 2020 growth %, 2020 vs 2019 growth % , these comparisons highlight the year-over-year growth at the monthly level.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/P%26L%20Statement%20by%20Months.png" class="center">

#### **P & L Year (Markets) Report** 

This report provides a year-wise financial summary for each market (country), including key metrics such as Net Sales, COGS (Cost of Goods Sold), Gross Margin, and Gross Margin %.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/P%26L%20Statement%20by%20Markets.png" class="center">

#### **Product Based Report**

This report highlights the top 10 products based on the percentage increase in their net sales from 2020 to 2021. It provides a clear comparison of product-level performance and growth trends over the year.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Product%20Based%20Report.png" class="center">

#### **Division Level Report** 

This report presents the net sales data for each division for the years 2020 and 2021, along with the growth percentage, helping to evaluate performance across divisions.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Division%20Level%20Report.png" class="center">

#### **Top and bottom products - QTY Report** 

This report highlights the top 5 and bottom 5 products based on the quantity sold, helping identify best-selling and underperforming products.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Top%20and%20bottom%20products%20-%20QTY%20Report.png" class="center">

#### **New products - 2021 Report** 

This report showcases the newly launched products by Atliq in 2021, along with their respective net sales performance.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/New%20Products%20-%202021%20Report.png" class="center">

#### **Top 5 countries Report** 

This report highlights the top 5 countries based on their net sales performance in 2021, helping identify the most revenue-generating markets.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Top%205%20countries%20Report.png" class="center">

#### **GM% (sub_zone) Report** 

This report tracks the Gross Margin Percentage (GM%) for each sub-zone, broken down by fiscal quarters (Q1–Q4) across the years 2019, 2020, and 2021.

<img src="https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/GM%20%25%20by%20Subzone%20Report.png" class="center">

### **Overall Report**

![Overall Report.gif](https://github.com/SouravBose2000/Excel-Sales-Analytics/blob/main/Resources/Overall.gif)

*******************
### **Project Outcome**

By using this sales analytics report — specifically the **Customer Performance Report** and the **Market Performance vs Target Report** — it will help in answering key business questions such as:
- Which customers (e.g., Amazon, Croma) contributed the most to sales in past years?
- What was the year-over-year performance trend for each customer?
- How did each customer perform during peak seasons like Diwali, New Year, or Christmas?
- If a particular customer demands higher discounts, will it still be profitable for us overall?
- Which customers are eligible for performance-based bonuses or exclusive product access?
- Did each market (e.g., India, USA) achieve its monthly or annual net sales targets?
- Which markets underperformed and by how much?
- Are there markets consistently outperforming targets that may need capacity expansion?
- Which markets can be prioritized for launching new products based on past performance?

By using this Finance Analytics Report — specifically the **P & L by Fiscal Years Report**, **P & L by Fiscal Months Report** and **P & L Year (Markets) Report** — it will help in answering key business questions such as:
- How is the company performing financially at a monthly and yearly level?
- What is the gross profit margin, and how has it changed over time?
- Are we meeting our P&L targets set by the Finance department?
- How much are we spending on cost of goods sold (COGS), and is it under control?
- Is the business generating enough profit to support expansion or new investments?
- How does our performance compare with our strategic financial vision?
- Are the regional finance teams aligned with central finance in terms of financial reporting and decisions?
- Can we use this report during business reviews and executive meetings to back up decisions with data?

Furthermore, these reports will help in answering numerous 'why' questions based on different business situations and decisions can be taken based on the data.
