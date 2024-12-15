# Business-Insights-360

AtliQ Hardware, a rapidly growing company, has decided to implement Data Analytics using Power BI for the first time to gain a competitive edge in the market and make data-driven decisions. This initiative aims to address stakeholders' critical questions across various business aspects, including finance, sales, marketing, and supply chain management.

As part of this project, I utilized advanced Power BI techniques, following the comprehensive Codebasics Power BI Course. The project involved designing dynamic dashboards and visualizations, enabling actionable insights for stakeholders.

Check out the course : [here](https://codebasics.io/)

Power BI live Dashboard :[click here](https://app.powerbi.com/view?r=eyJrIjoiYzIyYzRhNGMtN2Q4Mi00Y2E1LWI1MzctMTI2ZWZlMzRhMjlkIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9) 





𝗦𝗸𝗶𝗹𝗹𝘀 𝗛𝗶𝗴𝗵𝗹𝗶𝗴𝗵𝘁
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

✔ Expertise in Power BI, SQL, Excel, DAX, and DAX Studio (for optimizing reports).

✔ Proficient in data modeling, dashboard design, and KPI tracking.

✔ Specialized in delivering actionable insights for finance, sales, marketing, supply chain, and executive reporting.

✔ Skilled in Power BI Service for report publishing and personal gateways for data auto-refresh.


𝗟𝗲𝗮𝗿𝗻𝘁 𝗣𝗼𝘄𝗲𝗿𝗕𝗜 𝗧𝗲𝗰𝗵𝗻𝗶𝗾𝘂𝗲𝘀
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

✔ Creating calculated columns

✔ Creating measures using DAX language

✔ Data modeling for actionable insights

✔ Using bookmarks to switch between visuals

✔ Page navigation with buttons

✔ Creating date tables using M language

✔ Using KPI indicators for performance tracking

✔ Data validation techniques

✔ Power BI Service for report sharing

✔ Publishing reports to Power BI Service

✔ Setting up personal gateways for auto-refresh of data

✔ Sector-Specific Insights: Tailored analytics for finance, sales, marketing, and supply chain performance.


𝐁𝐮𝐬𝐢𝐧𝐞𝐬𝐬 𝐑𝐞𝐥𝐚𝐭𝐞𝐝 𝐓𝐞𝐫𝐦𝐬
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

✔ Gross Revenue

✔ Discounts and Allowances (Pre-Invoice Adjustments)

✔ Rebates and Credits (Post-Invoice Adjustments)

✔ Net Revenue

✔ Gross Profit Margin (GPM)

✔ Adjusted Net Sales

✔ Operating Profit

✔ COGS - Cost of Goods Sold

✔ YTD Metrics - Year-to-Date Performance

✔ YTG Projections - Year-to-Go Trends


𝗖𝗼𝗿𝗲 𝗧𝗲𝗰𝗵𝗻𝗶𝗾𝘂𝗲𝘀
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📌 Dynamic visuals and titles for tailored insights.

📌 Conditional formatting and data validation for high-quality reporting.

📌 Optimization of reports using DAX Studio.


𝗕𝘂𝘀𝗶𝗻𝗲𝘀𝘀 𝗦𝗲𝗰𝘁𝗼𝗿 𝗜𝗺𝗽𝗮𝗰𝘁
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

💼 Finance: Gross margin, net profit, and cost analysis.

💼 Sales: Revenue growth, YTD, and GM% tracking.

💼 Marketing: Campaign performance and ROI analysis.

💼 Supply Chain: Efficiency improvements and inventory optimization.

💼 Executive Reporting: Strategic dashboards for key decision-making.



# Company Background
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

AtliQ Hardware is a globally expanding enterprise specializing in the sale of computers and computer accessories. The company operates through three primary channels:

    Retailers
    Direct Sales
    Distributors

Despite its rapid growth and global reach, AtliQ Hardware recently encountered an unforeseen financial loss due to the decision to open a store in America. This decision was primarily driven by surveys, intuition, and limited Excel-based analysis. Meanwhile, competitors leveraged advanced analytics teams to drive data-backed decisions, creating a significant competitive disadvantage for AtliQ Hardware.

Recognizing this gap, AtliQ Hardware has initiated a transformational journey to build a robust data analytics team to deliver actionable insights and enable data-driven decision-making across critical business domains. This initiative is pivotal for the company to remain competitive and sustain its growth in the dynamic technology market.


# Project Objective
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The project commenced with a detailed kick-off session, where the scope and objectives were clearly defined. The primary goal is to empower AtliQ Hardware with a centralized analytics solution using Power BI to address stakeholders' pressing questions across key areas:

    Finance
    Sales
    Marketing
    Supply Chain

Through this project, AtliQ Hardware aims to transition from intuition-based decision-making to a robust, data-driven strategy, ensuring long-term success in the competitive landscape.

# Key Questions Before Starting the Dashboard
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
    1) What is the primary objective of this Power BI dashboard?
    2) How will project success be measured?
    3) What is the project timeline?
    4) Are stakeholders expecting a preview before the final release?
    5) What are stakeholders' goals and concerns for this project?
    6) Who will use the dashboard, and for what purpose?
    7) What are stakeholders’ expectations for the completed project?
    8) What risks could arise during development?
    9) What data and resources are required for this dashboard?
    10) Are there any stakeholder preferences for dashboard design or layout?

Following the project kick-off, the Data Engineering team provided the necessary datasets for the Data Analytics team to begin exploration.

# Dataset Overview
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
A clear understanding of available data is crucial before analysis. The dataset consists of dimension and fact tables stored in gdb041 and gdb056 databases.
gdb041:

    dim_customer:
        27 markets (e.g., India, USA, Spain)
        75 customers across markets
        2 platforms: Brick & Mortar, E-commerce
        3 channels: Retailer, Direct, Distributor

    dim_market:
        27 markets grouped into 7 sub-zones and 4 regions (APAC, EU, LATAM, nan)

    dim_product:
        Divisions:
            Peripherals & Accessories (P&A)
            PC (Notebook, Desktop)
            Networking & Storage (N&S)
        14 categories (e.g., Internal HDD, Keyboard) with multiple variants

    fact_forecast_monthly:
        Forecasted customer demand (start date as the monthly marker)
        Denormalized for analytical use, improving:
            Customer satisfaction
            Storage cost efficiency

    fact_sales_monthly:
        Similar to fact_forecast_monthly, but contains actual sold quantities.

gdb056:

    freight_cost: Travel and logistics costs per market and fiscal year
    
    gross_price: Gross prices linked to product codes
    
    manufacturing_cost: Manufacturing costs by product and year
    
    pre_invoice_deductions: Customer-specific pre-invoice deduction percentages by year
    
    post_invoice_deductions: Details of post-invoice deductions and other charges

# Importing Data into Power BI
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
The dataset is stored in a MySQL database. To import it into Power BI, connect to the database using the provided access credentials.

# Data Model
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data modeling serves as the foundation of any report, directly impacting its performance and accuracy. A well-structured data model ensures efficiency and reliability in visualizations, while poor modeling can degrade overall report performance.

In this project, we adhered to industry best practices and implemented a Snowflake Schema data modeling approach to optimize data organization and support effective analysis.
![image alt](https://github.com/Maheshmurari1/image/blob/3a0ec3e4707bfefe3224100e5ac14882b967df9c/Screenshot%202024-12-14%20220118.png)

# Dashboard Design
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Using the mock-ups provided, the team begins designing visuals and creating measures as needed.
Home Page

The Home Page serves as a navigation hub, allowing users to access specific sections by clicking the relevant buttons:

    Overview
    Financial Insights
    Revenue Performance
    Market Trends
    Operational Efficiency
    Leadership Dashboard
    Product Analytics
    Customer Support

#  Overview
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
👉 Ready to contribute impactful solutions to drive business growth.

https://github.com/user-attachments/assets/70447a3e-5359-4cd8-aea4-14d0436d54a3

# Finance
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://github.com/user-attachments/assets/cf489464-408d-4dac-9fe0-8c3dc7b9d5c3
# Sales 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://github.com/user-attachments/assets/ef5f389a-4930-436f-8299-2412f6e58a10
# Marketing
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://github.com/user-attachments/assets/ec71092d-ac2f-40d0-a0ad-f912807d5502
# Supply Chain
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://github.com/user-attachments/assets/5a9515bf-f5d9-4db0-8fef-900692b33051
# Executive 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://github.com/user-attachments/assets/948a2860-2b9c-4ff1-afdf-9a8f6589d2ed

# Power BI Certificate
Thrilled to share that I’ve earned a certification in Power BI, enhancing my skills in data visualization and business intelligence. Excited to apply these insights to real-world challenges.
Check for the Certificate : [Click here](https://codebasics.io/certificate/CB-49-344462)
