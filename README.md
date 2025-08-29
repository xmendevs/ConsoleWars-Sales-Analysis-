#  THE ConsoleWars (Sales Analysis)

<img width="2048" height="2048" alt="Gemini_Generated_Image_vacvb6vacvb6vacv" src="https://github.com/user-attachments/assets/39bda926-aceb-4312-a6b6-6cb46235a32d" /> 

### Table of Contents
- [Project Overview](#Project-Overview)
- [Problem Statement](#Problem-Statement)
- [Tools & Technologies](#Tools-&-Technologies)
- [Skills and Concept Demonostrated ](#Skills-and-Concept-Demonostrated)
- [Data Modelling](#Data-Modelling)
- [Data Sourcing](#Data-Sourcing)
- [Data Transformation](#Data-Transformation)
- [Visualization and Analysis](#Visualization-and-Analysis)
- [Conclusion](#Conclusion)


## Project Overview
This project involved the creation of a comprehensive and interactive sales dashboard using Power BI to analyze market performance and consumer behavior within the gaming console industry. The primary objective was to transform raw sales data into actionable business intelligence, providing a clear visual overview of key performance indicators (KPIs), market trends, and competitive dynamics.

## Problem Statement
A forward-thinking enterprise needs to understand its position in the highly competitive console market. By analyzing sales data, the company can identify its most profitable customer segments, understand geographical strengths, and track the performance of its key products. This analysis will guide strategic decisions, from marketing budget allocation to supply chain management

 The project aims to answer several key questions about the company's performance in the console market.

### Core Questions

* **Market Position**: How does our performance compare to that of our competitors, such as PlayStation, Nintendo, and Xbox?
* **Customer Insights**: Which customer segments are most profitable, and what are their purchasing behaviors?
* **Geographical Performance**: Which regions are our strongest markets, and where are the opportunities for growth?
* **Channel Effectiveness**: Is our online sales channel more effective than retail, and what is the exact split of sales between the two?
* **Operational Efficiency**: What is our game return rate, and does it indicate a potential issue with product quality or customer satisfaction?
* **Strategic Planning**: How do our sales trends fluctuate throughout the year, and how can we use this information for better inventory and marketing planning?

## Tools & Technologies

* Data Processing: Excel/ Power Query for data cleaning and transformation
* Data Visualization: Power BI (Interactive Dashboard)

## Skills and Concept Demonostrated 
The following Power Bi was incoporated:
* Data Cleaning
* Filtering & Sorting
* Calender Creation
* Calculated Field
* Measures
* Slicers
* Wire Framing
  
## Data Modelling

<img width="512" height="251" alt="image" src="https://github.com/user-attachments/assets/237686bc-138f-4654-b6cd-e1720abea5e8" />

### Model Analysis
The data model consists of two tables linked by a one-to-one relationship.

Gaming_Console_Sales_2025: This table contains both fact data (measures like Revenue and Marketing Budget) and dimension attributes (Console Brand, Customer Segment, Date, etc.). It acts as the central hub of the model.

ConsoleImages: This table is a dimension table, providing descriptive attributes related to the console brand.

The Star schema model was used in this Project.

## Data Sourcing 
The synthetic Data set was downloaded online from Kaggle.com in other to put my skills on Descriptive analysis into practice and uncover Trends and Patterns it covers years ranging from 2020 - 2025

## Data Transformation 
To prepare the data for analysis, the following data transformation steps were taken using **Power Query** in Power BI:

1.  **Data Source Connection**: The process began by connecting to the raw data files, likely a CSV or Excel spreadsheet containing all the sales records.

2.  **Merging Queries**: The `ConsoleImages` table was **merged** with the main `Gaming_Console_Sales_2025` table using `Console Brand` as the common key. This step simplified the data model by combining two related tables into a single, comprehensive table, which is a best practice for a star schema.

3.  **Data Cleaning**: Several cleaning tasks were performed to ensure data quality and accuracy:
    - **Removed Duplicates**: Duplicate rows were removed to prevent inaccurate calculations.
    - **Handled Errors and Missing Values**: Null or error values in key columns were addressed to maintain data integrity.

4.  **Data Type Conversion**: The data types for all columns were validated and converted to the correct format. For example, `Revenue ($)` was set to a decimal number, `Units Sold` was set to a whole number, and `Date` was converted to a proper date format.

5.  **Created Calculated Columns**: New columns were created to enhance analysis. For example, columns for `Year`, `Quarter`, and `Month` were derived from the `Date` column to enable time-based analysis.

6.  **Loaded to Data Model**: The final, cleaned, and transformed dataset was loaded from the Power Query Editor into the Power BI data model, where relationships were established and **DAX measures** were created to perform the final calculations for the dashboard's KPIs.

## Visualization and Analysis

The visualization of this porject consist of one page
you can interactive with the dashboard [here](https://app.powerbi.com/groups/3dca1cef-7993-44e0-bcb9-d0ee6f4a8fc0/reports/244b1ccb-fdea-4dac-a458-3f652ad52183/0d64f154a420d0ea7670?experience=power-bi)
- Slicers for different years are at the top of the page
- Also click on any part of the image to interact with other parts of the Dashboard.

### Analysis
  <img width="287" height="361" alt="image" src="https://github.com/user-attachments/assets/9da368c1-4a7f-4f1e-a18b-feef23c1b37c" /> | Dominance of Online Sales: Online channels accounted for the majority of sales, representing 57.1% of total units sold, while retail made up 42.9%. This highlights the importance of a strong e-commerce strategy.

---

<img width="342" height="374" alt="image" src="https://github.com/user-attachments/assets/c517fd40-e121-4cb7-bc87-094f66e4dc40" />| Customer Segmentation: The Teens customer segment was the top performer, contributing 40.3% of sales. This group presents the most significant revenue opportunity.

---

<img width="601" height="334" alt="image" src="https://github.com/user-attachments/assets/e5d3c44b-7001-406a-ad1e-aaede3ad8d44" />
Geographical Performance: Africa leads in total revenue at ₦4.2M, followed by Asia at ₦3.2M. This indicates a strong market presence in these regions.

---

<img width="677" height="431" alt="image" src="https://github.com/user-attachments/assets/95ba2cea-34c4-41c9-88d9-13d0b6812a4d" />
Quarterly Trends: Sales experienced a notable dip in Qtr 2 before a significant recovery and peak in Qtr 4, likely driven by holiday sales and new console releases. This trend is consistent across both revenue and units sold.

---

<img width="631" height="220" alt="image" src="https://github.com/user-attachments/assets/a267365a-2742-48c5-b47f-04428a8cd000" />
Top Performing Brands: The PlayStation 5 sold the most units with 99K, followed by the Nintendo Switch at 85K and the Xbox Series X at 65K. This confirms the PlayStation's leading market position.

---

 <img width="123" height="148" alt="image" src="https://github.com/user-attachments/assets/b042b5d9-eae5-4f76-9498-6c2a4ee8c0ca" />
Operational Metrics: The company maintained a low game return rate of 4.67%, indicating high customer satisfaction and a quality product lineup

---

## Conclusion

This data analysis project successfully transformed raw sales data into a comprehensive and actionable Power BI dashboard. By creating a unified view of market performance, the project provided key insights into customer behavior, geographical strengths, and brand performance. The analysis confirmed the dominance of **online sales** and the **Adult customer segment**, and highlighted the significant market presence in **Africa**. Furthermore, the project identified crucial quarterly sales trends, enabling better planning for the peak holiday season. Ultimately, this report demonstrates the power of data visualization and analytics in guiding business strategy and unlocking growth opportunities.


## Recommendations

Based on the findings from this analysis, here are key recommendations to drive strategic growth:

1.  **Optimize the E-commerce Strategy**: Given that online sales account for 57.1% of units sold, the company should invest further in its digital storefront and online marketing. This includes improving the user experience, enhancing targeted advertising campaigns, and offering exclusive online promotions to capitalize on this leading channel.
2.  **Target the Adult Demographic**: The **Adult** segment is the highest-grossing customer group. Marketing efforts and product development should be tailored to this demographic's preferences. Consider creating content, partnerships, and product bundles that appeal directly to this lucrative market.
3.  **Expand and Capitalize on High-Growth Regions**: The data shows **Africa** as a top-performing region. The company should explore opportunities for expansion, partnerships, and localized marketing efforts in this and other high-growth areas to solidify and grow its market share.
4.  **Enhance Holiday Season Planning**: The significant sales peak in Q4 requires proactive planning. Recommendations include increasing inventory in Q3, launching strategic marketing campaigns ahead of the holiday rush, and ensuring robust supply chain management to meet the surge in demand.
5.  **Refine the Data Model**: To ensure future scalability and performance, the data model should be refined. Merging the `Gaming_Console_Sales_2025` and `ConsoleImages` tables into a single, clean fact table will simplify the model and improve report performance.

<img width="2000" height="2000" alt="image" src="https://github.com/user-attachments/assets/8f7232f2-e8b0-4425-b26a-5b7dd1e5e745" />





