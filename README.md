# Project: Customer-Segmentation-and-Analysis
## Introduction:
In this project, I employ Python data libraries (Pandas, Matplotlib, Plotly) and the K-Means clustering algorithm to wrangle retail data, perform exploratory data analysis(EDA) and undertake a customer segmentation analysis using RFM (Recency, Frequency, Monetary) analysis to understand and unravel the intricacies of customer behaviour on a UK based and registered non-store online retail platform.

## Dataset Overview
The dataset used for this project encompasses a diverse array of more than 500K transactions, capturing the interactions of customers with the online retail platform. Features such as transaction dates, purchase amounts, and customer identifiers form the foundation for a comprehensive exploration of customer dynamics.
The following is a description of the columns that make up the dataset. For each data record, there are 8 variables.
1. __InvoiceNo__: This is a 6-digit integer number, uniquely assigned to each transaction.
                  If the code starts with a 'C', it indicates a cancelled transaction.
   
2. __stockCode__: This is a 5-digit integer number uniquely assigned to a distinct product on the online retail store.

3. __Description__: Product(item) name.

4. __Quantity__: The count or quantities of each product(item) per transaction.

5. __InvoiceDate__: Invoice date and time. Day and time when each transaction was generated.

6. __UnitPrice__: Product price per unit in pound sterling.

7. __CustomerID__: 5-digit number uniquely assigned to each customer.

8. __Country__: Country where each customer resides.

## Project Structure
This project comprises three stages:
### 1. Stage One: Data Wrangling (Cleaning & Preparation)
This is the first stage of the project where I focus on cleaning and preparing the data from a UK-based and registered non-store online retail for the Exploratory Data Analysis (EDA) stage and to undertake Customer Segmentation and Analysis. In this stage of the project, I undertake the following tasks;
- Removing duplicate values and entries
- Removing all null values
- Correcting column data types
- Correcting data anomalies
- Formatting data values
  
__NB:__ In this stage, comments have been included in each code cell to guide users and viewers through the data-wrangling process.
For proper viewing and rendering of the interactive visualizations, please click on the following link:
[Customer Segmentation Analysis - Data Wrangling (Cleaning and Preparation)](https://nbviewer.org/github/GameliKofiJerome/Customer-Segmentation-and-Analysis/blob/main/Customer%20Segmentation%20Analysis%20-%20Data%20Wrangling%20%28Cleaning%20%26%20Preparation%29.ipynb)

### 2. Stage Two: Exploratory Data Analysis (EDA)
This is the second stage of the project where I delve into the cleaned sales data from the data wrangling stage to explore and understand the key aspects of the data. I use interactive visualizations to communicate key insights and trends, as well as summary statistics to highlight key aspects of the dataset, helping stakeholders understand the nature of the data.
By answering questions about the data, I derived some key performance indicators (KPIs). These key questions are as follows:
- What proportion of transactions were captured as either `sale` or `canceled`?
- What was the trend in transactions made over the recorded period?
- From which countries were the most or least transactions recorded with respect to transaction type (sale or canceled)?
- During which time of day (morning, afternoon, evening) were transactions made?
- From which country did the online retail store have the most or least customers?

__For each of the above questions, the key insights derived are found below each chart used to visualize the dataset result that explains the findings.__

For proper viewing and rendering of the interactive visualizations, please click on the following link:
[Customer Segmentation Analysis - Exploratory Data Analysis](https://nbviewer.org/github/GameliKofiJerome/Customer-Segmentation-and-Analysis/blob/main/Customer%20Segmentation%20Analysis%20-%20Exploratory%20Data%20Analysis.ipynb)


### 3. Stage Three: RFM (Recency, Frequency, Monetary) Analysis
In this final stage of the customer segmentation & analysis project, I delved into the dataset(cleaned) of the online retail store to unravel the intricacies of customer behaviour. By leveraging the K-Means Clustering algorithm and the powerful RFM (Recency, Frequency, Monetary) analysis, I aimed to distil valuable insights that could profoundly impact business strategies and enhance customer-centric decision-making.
The dataset encompasses a diverse array of almost 400K transactions, capturing the interactions of customers on the online retail platform. Features such as transaction dates(InvoiceDate), purchase amounts(UnitPrice), product quantity, stock code and customer identifiers form the foundation for a comprehensive exploration of customer dynamics.
The following are the objectives for this stage of the project:
1. Segmentation for Potential Targeted Marketing:
    - How can customers be categorized into distinct segments based on their recency, frequency, and monetary contributions?
    - What insights can these segments provide to guide marketing strategies for improved customer engagements?

2. Identifying High-Value Customers:
    - Can we identify or pinpoint high-value customers who contribute significantly to the business's revenue?
    - What patterns in recency, frequency, and monetary metrics characterize these high-value customers?
  
3. Understanding the correlation between RFM metrics:
    - How do recency and purchasing frequency affect the monetary contributions of each customer segment?

4. Customizing Communication Strategies:
    - How can communication strategies be customized for different customer segments to enhance the overall customer experience
    - What personalized approaches can be adopted based on the identified RFM segments?
   
For proper viewing and rendering of the interactive visualizations, please click on the following link:
[Customer Segmentation Analysis - K-Means Clustering and RFM Analysis](https://nbviewer.org/github/GameliKofiJerome/Customer-Segmentation-and-Analysis/blob/main/Customer%20Segmentation%20Analysis%20-%20K-Means%20Clustering%20and%20RFM%20Analysis.ipynb)

## Conclusion
### Summarized Key Insights from Customer Segmentation & Analysis
1. Proportion of Transaction Types:
    - Cancelled transactions constitute a small percentage (5.12%) but accumulate a significant total amount (471,742.31).
    - Sale transactions dominate, comprising 94.9% of all transactions, with a total amount of 8,737,061.14.
2. Monthly and Yearly Trends in Transactions:
    - December 2010 had the only recorded sales, totalling 565,145K, outperforming December 2011.
    - Sales in 2011 varied monthly, with a peak in November (1.137 million).
    - Cancelled transactions were notable in December 2010 and peaked in December 2011 (174,076K).
3. Countries with the Most Sales and Canceled Transactions:
    - Top 10 countries for sale transactions: the United Kingdom led in both the number of transactions (348,800) and total amount (7.2 million).
    - Bottom 10 countries for sale transactions: Saudi Arabia had the lowest transactions (9) and the total amount (145.92).
    - Top 10 countries for cancelled transactions: the United Kingdom led with 7,217 transactions and 440,301.34 total amount.
4. Time of Day Analysis:
    - Sales for 2010 occurred mainly in the afternoon in December.
    - In 2011, mornings dominated sales across months, with occasional afternoon and evening peaks.
5. Countries with Most Customers:
    - Top 10 countries with the most customers: United Kingdom had the highest (3,943), while Austria had the lowest (11).
    - Bottom 10 countries with the least customers: Bahrain had the highest among the bottom group (2), while several countries had the lowest (1).
    
### Emphasized Value of Customer Segmentation:
  - Informed Decision-Making: Customer segmentation allows the online retail store to make informed decisions based on transaction types, trends, and customer distribution.
  - Targeted Marketing: Understanding customer behaviour enables targeted marketing strategies, optimizing efforts and resources.
  - Risk Mitigation: Identifying trends in cancelled transactions helps in implementing risk mitigation strategies.
  - Customer Retention: Recognizing peak sales times informs strategies to enhance customer engagement and retention.
  - Global Strategy: Knowing customer distribution by country aids in tailoring strategies for different markets.
    
Customer segmentation, as revealed by the analysis, is a powerful tool for the online retail store, guiding strategic decisions and enhancing overall business performance.

__NB:__ It must be noted that the currency value of all transaction amounts in this project is the pound sterling.

__NB:__ 
- HTML files of the Exploratory Data Analysis and RFM Analysis have been included. Download the files onto your local device and open them in your browser. The files serve as reports for both stages and are made up of interactive visualizations. They do not show the code cells.
- PDF files of both the Exploratory Data Analysis and RFM Analysis have also been included.
- For proper viewing and rendering of the interactive visualizations in the `ipynb` files, please click to open the following links:
  - [Customer Segmentation Analysis - Exploratory Data Analysis](https://nbviewer.org/github/GameliKofiJerome/Customer-Segmentation-and-Analysis/blob/main/Customer%20Segmentation%20Analysis%20-%20Exploratory%20Data%20Analysis.ipynb)
  - [Customer Segmentation Analysis - K-Means Clustering and RFM Analysis](https://nbviewer.org/github/GameliKofiJerome/Customer-Segmentation-and-Analysis/blob/main/Customer%20Segmentation%20Analysis%20-%20K-Means%20Clustering%20and%20RFM%20Analysis.ipynb)
