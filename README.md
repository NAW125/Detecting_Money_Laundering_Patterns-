# Detecting Money Laundering Patterns Across Global Financial Transactions

## Table of Contents
1. [Overview](#overview)
2. [The Dataset](#dataset-description)
3. [Key Objectives](#key-objectives)
4. [Methodology](#methodology)
5. [Analysis & Findings](#analysis--findings)
6. [Dashboard Features](#dashboard-features)
7. [AI Tool Integration](#ai-tool-integration)
8. [Ethical & Legal Considerations](#ethical--legal-considerations)
9. [Challenges & Reflections](#challenges--reflections)
10. [Assessment Criteria](#assessment--criteria)


##  1. Overview
### 1.1 Problem Statement

Money laundering is a significant and growing global issue that directly funds organized crime and terrorism. While the true scale of money laundering is difficult to quantify, the United Nations Office on Drugs and Crime (UNODC) estimates that between 2% and 5% of global GDP is laundered each year—equivalent to EUR 715 billion to 1.87 trillion annually.

To combat this, banks and financial institutions worldwide are subject to regulations at both national and international levels. The responsibility to detect and report money laundering activities falls on corporate institutions globally, although the effectiveness of these efforts varies.

When institutions fail to comply with anti-money laundering (AML) regulations, the consequences can be severe. In June 2025, for example, the Monetary Authority of Singapore issued a record fine of $1.6 billion in a high-profile laundering case that damaged the city's financial reputation.

Beyond financial penalties, money laundering poses a direct threat to the profitability and reputation of institutions and contributes to long-term societal harm by enabling criminal networks that destabilize communities worldwide.

In the United Kingdom, the Proceeds of Crime Act 2002 requires financial institutions to implement risk-based customer due diligence approach and take proactive measures to prevent their services from being used for money laundering or terrorist financing.
This project investigates synthetic financial transaction data to identify patterns indicative of money laundering, drawing on datasets that span multiple countries, industries, and transaction types.

## 2. Dataset 
This project explores synthetic financial transaction data, modelled on real data to detect patterns consistent with money laundering activity. Using data spanning multiple countries across the world, industries, and transaction types, we apply statistical methods, risk scoring, and machine learning models to identify patterns of behavior associated with money laundering. 
The objective is to identify anti-money laundering (AML) insights and recommendations by highlighting suspicious transaction profiles with a view to informing and improving financial compliance workflows.
All data used has been generated for research purposes mimicking  the complexity and structure of real-world financial transactions.

### 2.1 Dataset Source
https://www.kaggle.com/datasets/waqi786/global-black-money-transactions-dataset

### 2.2 Dataset 
Money_Laundering_Dataset_.csv (10,000 records X 14 columns)


### 2.3 Dataset Columns

| Column Name                    | Description                                                                 |
|-------------------------------|-----------------------------------------------------------------------------|
| **Transaction ID**            | A unique identifier for each financial transaction.                        |
| **Country**                   | The country where the transaction was initiated.                           |
| **Amount (USD)**              | The monetary value of the transaction in U.S. dollars.                     |
| **Transaction Type**          | The nature of the transaction (e.g., deposit, withdrawal, transfer).       |
| **Date of Transaction**       | The date on which the transaction occurred.                                |
| **Person Involved**           | An anonymised label representing the individual associated with the transaction. |
| **Industry**                  | The industry sector associated with the person or organisation involved.   |
| **Destination Country**       | The country where the funds were sent or intended to be received.          |
| **Reported by Authority**     | Indicates whether the transaction was reported to a regulatory or financial authority. |
| **Source of Money**           | The declared or inferred origin of the funds involved in the transaction.  |
| **Money Laundering Risk Score** | A numerical or categorical score assessing the potential risk of money laundering. |
| **Shell Companies Involved**  | Indicates whether shell companies were linked to the transaction.          |
| **Financial Institution**     | An anonymised identifier for the financial institution handling the transaction. |
| **Tax Haven Country**         | Specifies whether the transaction is connected to a known tax haven jurisdiction. |


*Date of transactions - transactions span a two year period from 2013 - 2014. We will carry out a data shift to 2023/ 2024 during the ETL process to enable the analysis of any seasonality variations within the dataset. 

## 3. Key Objectives 

- Identify behavioural patterns and proxy patterns linked to money laundering. 
- Test key hypotheses using the data set 
Visualise findings through interactive Tableau dashboards
- Translate insights into actionable business recommendations.

## 4. Business Requirements 
This project supports stakeholder decision-making with clear, data-driven insights into the drivers patters of behaviour around money laundering. 


## 5. Key Business Goals
Identify adequate processes and procedures to better compy with anti-money laudering regulations, at the domestic and international level. 

## 5. Hypothesis 

| # | Hypothesis | Business Question | Why it Matters | Type of Analysis |
|---|--------------------------------------|-------------------------|----------------|-------------------|
| 1 | Cross-border transactions are more often associated with legal sources of funds compared to domestic transactions. | Are intra-country transactions more likely to be illegal, costing the business money? | Consequences for the business in terms of reputation, government fines, profitability, and shareholder satisfaction. | Comparative |
| 2 | Illegal transactions are more common in high-risk sectors such as Casinos and Luxury Goods. | Can we identify industries where transactions are more likely to be fraudulent? | Enables more effective monitoring of high-risk sectors to prevent money laundering. | Comparative |
| 3 | Cross-border transactions involving tax haven countries are more likely to be associated with illegal sources of money. | Should transactions involving tax havens be flagged as higher risk? | Allows AML teams to focus efforts on transactions involving known high-risk jurisdictions. | Comparative |

## 5. Methodology 
### 5.1  Project Plan
A structured data analysis workflow ensured traceability from business objectives to actionable insights.
### High-Level Steps
**- Data Collection**  – Source from Kaggle

**- Data Processing** – Clean, transform, encode
Exploratory Data Analysis and hypothesis testing.

**- Visualisations** – Built with Tableau

**- Tools**
Python in VS Code (ETL and feature engineering)

GitHub (Version Control)

Tableau (Interactive Dashboard and visualisation)

