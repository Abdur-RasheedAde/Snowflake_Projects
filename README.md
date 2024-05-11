# Cricket Analaysis Project with Snowflake

![Slide1](https://github.com/Abdur-RasheedAde/Snowflake_Projects/blob/main/SNOWFLAKEHOME.png)

##  Introduction
This is a Big Data-Data Engineering (End-to-end) project exploring snowflake cloud. The project injest a json file, perform all necessary ETL processes and created a Snowflake dashboard to visualise the data. 

## Data Source:
The data used is a Cricket World Cup match in 2023 which comes in a json file injested directly from a folder;  
* Cricket World Cup Match in 2023 [Downloadjsonfilehere](https://drive.google.com/drive/folders/1ls9ST-q6c2fCZZOuaC8Bd5lugrTKbVIE?usp=drive_link)

## DE Technical Skills:
+ Schema Creation
+ Data Injestion
+ Data Warehousing
+ Extract, Transform and Load (ETL) process
+ Flattering of JSON file into a Table
+ Data Modelling (Fact and Dimention table)
+ Data Visualization - dashboard
+ Feedback and Continuous Improvement
  
## Data Engineering Process
1. Creation of database and 4 Schemas: A database (DB) known as CRICKET is created with 4 Schemas (LAND, RAW, CLEAN and CONSUMPTION) for proper logical description and arrangement of the DB. The Star-schema was eventually used in Data Modelling so as to give the datawarehouse a legible understading (get the code here)[] 
2. Data Injestion and Loading: Data is injested into the LAND schema and reloaded into the RAW schema (access the code here)[]
3. njest Data into the RAW Schema
To optimize the performance of the data model, a calendar table was created using the DAX function. The data model follows a star schema with one fact table and three dimension tables. The dimension tables have PRIMARY KEYS that connect to the corresponding FOREIGN KEYS in the fact table, forming a one-to-many relationship between each dimension table and the fact table. The diagram below shows the data model.  
<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/Data%20Modelling.PNG" width=50% height=50%>

## Report Design and Visualization
The Report Canvas was designed in Power Point and imported to PowerBI as canvas background. Here is a sample of the slide in Power Point   
<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/Slide2.PNG" width=50% height=50%>  
5 pages were created; Home, Consolidated, Stationery, Cosmetics and Electronics. 
_Home_ page is the landing page while _Consolidated_ has the general report without filter while other pages has filtered reports accroding to their page name.
On each page, the new card visual is used to hold Total Sales, Gross Sales and Profit, Line Chart is used for the series analysis while a column and bar chart are adopted for the Continental and Country analysis respectively. The last image is the button for page navigation. 

| Visuals             |  Visuals |
:-------------------------:|:-------------------------:
<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/Card1.PNG" width=90% height=90%>|<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/button1.PNG" width=40% height=40%> 
<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/columnbarchart.PNG" width=60% height=60%> |<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/Linechart.PNG" width=100% height=100%> 

## Analytics and Insights
The data analysis revealed that;

1. There is a zig-zag trend of profit across the months, however, October records the highest profit of ($3.74M) which is 15% of the total profit and April records the least profit of ($1.4M), 6% of total profit
2. There exist an increase in profit from 2013 to 2014 with a ration of 4:6
3. Q4 record the highest profit of ($8.4M) with Q1 with the lowest ($5M), this shows steady increase in profit across the quarter from 1 to 4
4. The most and least profitable product category are Stationery and Cosmetics which amounts to 44% and 28% of the total profits respectively 
5. By region continent is intended, therefore Haut supermarket makes the most sales from America region ($98M) with 47% of the total Gross Sales
6. This is achieved with the help of the slicer; which shows that product with discount result to 96% of the total Gross sales while only 4% don't have discount, with **High** band of discount amounting to 41% of the Gross Sales
7. Africa pull 9% of the total Gross sales and 6% of the total Profit from the 202,286 Units solds from South Africa and Nigeria. This is can be visualised when clicking on Africa in the column chart 
8. France is the most profitable Country among the Haut Stores with 20% ($4.9M) of the total profit

![ConsolidatedDashboard](https://github.com/Abdur-RasheedAde/Haut_Sales_Analysis/blob/main/Page2Consolidated.PNG)

## Conclusions and Recommedations

1. Haut needs to conduct market analysis to increase sales in Q1 and Q2 and offer seasonal products that appeal to customers in the first half of the year
2. Haut’s management should continue their market strategy that leads to higher profits and better customer satisfaction
3. The cosmetics product category demands more research and development to boost its sales and profitability
4. Promotions (discounts) drive most of the sales in Haut stores, making them competitive in the dynamic market. Therefore, other promotional and marketing strategies should be implemented to enhance sales and profit
5. Products in Africa and China stores should be tailored to the specific needs of these markets through careful research

## Deployment to Power BI Service
This Report is deployed to Power BI service from my Microsoft developer account and publish to the web for everyone to have access to it.
[HautSupermarketAnalysis](https://app.powerbi.com/groups/me/reports/66ab0071-4b25-41c8-99fd-fd006603aacd/ReportSection6239a8326550e132bae6?ctid=32796be2-60fb-4da2-8d26-06e5938e6e6b&experience=power-bi)  

To Open a developer Microsoft account, kindly check this article [OpenMicrosoftdeveloperaccount](https://techcommunity.microsoft.com/t5/educator-developer-blog/register-for-microsoft-365-and-power-apps-developer-account-with/ba-p/3490280)

Thanks for taking time to go through this report! 🤝
