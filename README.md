# Project: Customer-Segmentation-and-Analysis
## Introduction:
In this project I employ Python data libraries (Pandas, Matplotlib, Plotly) and K-Means clustering algorithm to wrangle retail data, perform exploratory data analysis(EDA) and undertake a customer segmentation analysis using RFM analysis to understand and unravel the intricacies of customer behavior on a UK based and registered non-store online retail platform.

## Dataset Overview
The dataset used for this project encompasses a diverse array of more than 500K transactions, capturing the interactions of customers with the online retail platform. Features such as transaction dates, purchase amounts, and customer identifiers form the foundation for a comprehensive exploration of customer dynamics.
The following is a description of the columns the make up dataset. For each data record, there are 8 variables.
1. __InvoiceNo__: This is a 6-digit integer number, uniquely assigned to each transaction.
                  If code starts with a 'C', it indicates a cancelled transaction.
   
2. __stockCode__: This is a 5-digit integer number uniquely assigned to distinct product on the online retail store.

3. __Description__: Product(item) name.

4. __Quantity__: The count or quantities of each product(item) per transaction.

5. __InvoiceDate__: Invoice date and time. Day and time when each transaction was generated.

6. __UnitPrice__: Product price per unit in pound sterling.

7. __CustomerID__: 5-digit number uniquely assigned to each customer.

8. __Country__: Country where each customer resides.

## Project Structure
This project comprises of three stages:
### 1. Stage One: Data Wrangling (Cleaning & Preparation)
This is the first stage of the project where I focus on cleanimg and preparing the data from a U.K based and registered non-store online retail for the Exploratory Data Analysis (EDA) stage and to undertake Customer Segmentation and Analysis. In this stage of the project, I undertake the following tasks;
- Removing duplictae values and entries
- Removing all null values
- Correcting column data types
- Correcting data anomalies
- Formatting data values
__NB:__ In this stage, comments have been included in each code cell to guide users and viewers through the data wrangling process.

### 2. Stage Two: Exploratory Data Analysis (EDA)
This is the second stage of the project where I delve into the cleaned sales data from the data wrangling stage to explore and understand the key aspects of the data. I use interactive visualizations to communicate key insights and trends, as well as summary statistics to highlight key aspects of the dataset, helping stakeholders understand the nature of the data.
By answering questions on the data, I derive some Key Performance Indicators (KPIs). These key questions are as follows:
- What proportion of transactions were captured as either `sale` or `canceled`?
- What was the trend in transactions made over the recorded period?
- From which countries were the most or least transactions recorded with respect to transaction type (sale or canceled)?
- During which time of day (morning, afternoon, evening) were transactions made?
- From which country did the online retail store have the most or least customers?
  
__For each of the above questions, the key insights derived is found below each chart used to visualize the dataset result that explains the findings.__

### 3. Stage Three: RFM (Recency, Frequency, Monetary) Analysis
In this final stage of the customer segmentation & analysis project, I delved into the dataset(cleaned) of the online retail store to unravel the intricacies of customer behaviour. By leveraging the K-Means Clustering algorithm and the powerful RFM (Recency, Frequency, Monetary) analysis, I aimed to distill valuable insights that could profoundly impact business strategies and enhance customer-centric decision-making.
The dataset encompasses a diverse array of almost 400K transactions, capturing the interactions of customers on the online retail platform. Features such as transaction dates(InvoiceDate), purchase amounts(UnitPrice), product quantity, stock code and customer identifiers form the foundation for a comprehensive exploration of customer dynamics.
The folowing are the objectives for this stage of the project:
1. Segmentation for Potential Targeted Marketing:
    - How can customers be categorized into distinct segments based on thier recency, frequency, and monetary contributions?
    - What insights can these segments provide to guide marketing strategies for improved customer engagements?

2. Identifying High-Value Customers:
    - Can we identify or pinpoint high-value customers who contribute significantly to the business's revenue?
    - What patterns in recency, frequency, and monetary metrics characterize these high-value customers?
  
3. Understanding the correlation between RFM metrics:
    - How does recency and purchasing frequency affect monetary contributions of each customer segment?

4. Customizing Communication Strategies:
    - How can communication strategies be customized for different customer segments to enhance the overall customer experience
    - What personalized approaches can be adopted based on the identified RFM segments?

## Conclusion
### Summarized Key Insights from Customer Segmentation & Analysis
1. Proportion of Transaction Types:
    - Cancelled transactions constitute a small percentage (5.12%) but accumulate a significant total amount (471,742.31).
    - Sale transactions dominate, comprising 94.9% of all transactions, with a total amount of 8,737,061.14.
2. Monthly and Yearly Trend in Transactions:
    - December 2010 had the only recorded sales, totaling 565,145K, outperforming December 2011.
    - Sales in 2011 varied monthly, with a peak in November (1.137 million).
    - Cancelled transactions were notable in December 2010 and peaked in December 2011 (174,076K).
3. Countries with Most Sales and Canceled Transactions:
    - Top 10 countries for sale transactions: United Kingdom led in both the number of transactions (348,800) and total amount (7.2 million).
    - Bottom 10 countries for sale transactions: Saudi Arabia had the lowest transactions (9) and total amount (145.92).
    - Top 10 countries for canceled transactions: United Kingdom led with 7,217 transactions and 440,301.34 total amount.
4. Time of Day Analysis:
    - Sales for 2010 occurred mainly in the afternoon in December.
    - In 2011, mornings dominated sales across months, with occasional afternoon and evening peaks.
5. Countries with Most Customers:
    - Top 10 countries with the most customers: United Kingdom had the highest (3,943), while Austria had the lowest (11).
    - Bottom 10 countries with the least customers: Bahrain had the highest among the bottom group (2), while several countries had the lowest (1).
    
### Emphasized Value of Customer Segmentation:
  - Informed Decision-Making: Customer segmentation allows the online retail store to make informed decisions based on transaction types, trends, and customer distribution.
  - Targeted Marketing: Understanding customer behavior enables targeted marketing strategies, optimizing efforts and resources.
  - Risk Mitigation: Identifying trends in cancelled transactions helps in implementing risk mitigation strategies.
  - Customer Retention: Recognizing peak sales times informs strategies to enhance customer engagement and retention.
  - Global Strategy: Knowing customer distribution by country aids in tailoring strategies for different markets.
    
Customer segmentation, as revealed by the analysis, is a powerful tool for the online retail store, guiding strategic decisions and enhancing overall business performance.

__NB:__ It must be noted that the currency value of all transaction amounts in this project is the pound sterling.
