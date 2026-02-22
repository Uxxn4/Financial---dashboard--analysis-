# Financial---dashboard--analysis-
Financial analysis and interactive dashboard using tableau 



#


## Dashboard Preview 
![ Dashboard 1 ] (Dashboard Screen 1.png)

![ Dashboard 2 ] (Dashboard Screen 2.png)



















#




Project Overview 

This is a financial analysis and dashboard for Apple Inc. (AAPL), one of the most valuable companies. the analysis is trying to answer how has Apple performed financially and in the stock market over time. 






# 


Data Scource 

The data Used in this analysis comes from two primary sources. the first is Kaggle, which provided historical stock market data Apple covering daily trading activity from December 1980 to January 2026. This data include price metrics such as open, high , low, and closing price. The second The second source is Apple's official 10-K Annual Report, published on the Apple Investor Relations website. This report provided segment-level revenue data broken down by product category — iPhone, Mac, iPad, Services, and Wearables & Other — as well as geographic revenue data segmented into five regions: Americas, Europe, Greater China, Japan, and Rest of Asia Pacific. This financial data spans fiscal years 2023 through 2025 and is reported in millions of US dollars.







# 


Steps & Methodology

The project beginning with data cleaning and transformation in Python, followed by visualization in Tableau. The Kaggle stock dataset required several cleaning steps: converting the date column from a string object to a proper datetime format, checking for duplicate records and rows with missing values. Also ensuring the daily high price was never below the daily low.  The quarterly financial dataset required a different approach. It was discovered that revenue figures were recorded annually rather than quarterly, meaning the same annual value appeared repeated across all four quarters of each fiscal year. Rather than dividing these values to estimate quarterly figures — which would introduce inaccuracy - the data was restructured to treat revenue as annual, and duplicate quarterly rows were removed, resulting in one clean record per fiscal year per product category.
For visualization purposes, revenue data was reshaped from wide format, where each product had its own column, to long format with a single product column and a single revenue column. This transformation was to enable Tableau to build stacked and grouped charts. Regional revenue data from the 10-K report was manually entered in Python before being exported as a CSV file for use
In Tableau. 







# 


Key Insights

Apple's stock price has experienced long-term growth, rising from under one dollar in the early 1980s to over two hundred and fifty dollars by 2025. Regards Apple's revenue, while the iPhone remains the dominant revenue source, contributing over 50% of total revenue, the Services  has grown and now represents the second-largest contributor. From a regional perspective, the Americas remain Apple's largest market, generating $178 billion in fiscal year 2025. However, Greater China being the only region to record negative growth in both 2024 and 2025, declining 8% and 4% respectively. Japan showed the strongest growth in 2025 at 15%, though it remains a relatively smaller market in absolute terms.
For a stakeholder, the key recommendation would be to monitor the Services revenue closely, as it represents Apple's most promising long-term growth engine. Additionally, the declining trend in Greater China warrants strategic attention. 








# 


Assumptions & Limitations

The quarterly revenue figures in the Kaggle dataset were found to be annual totals repeated across quarters, which limited the ability to do seasonality trend analysis. As a result, revenue analysis was done at the annual level only. having a quarter revenue would allow me to invastigate the iPhone launch cycles. 
The regional revenue data was sourced manually from the 10-K report and covers only fiscal years 2023 through 2025. This limits the historical depth of geographic analysis compared to the stock data. Additionally. 








# 



# Future Work 


There is a space to include a ML model to predict stock price, revenue, product growth and regional performance 
