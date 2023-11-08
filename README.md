# Lending Club Case Study

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Analysis Approach](#analysis-approach)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [TO-DO](#todo)
* [Contact](#contact)


## General Information

### Problem  introduction

A consumer finance company specializes in lending various types of loans to urban customers and faces the challenge of making informed decisions regarding loan approvals. The company's primary concern is managing two types of risks associated with loan approvals:
1. Risk of Loss due to Non-Approval: If the applicant is likely to repay the loan, not approving the loan results in a loss of potential business for the company.


2. Risk of Default: If the applicant is not likely to repay the loan and is likely to default, approving the loan may lead to a financial loss for the company.

### Business Objective

The primary business objective is to use Exploratory Data Analysis (EDA) and risk analytics to identify patterns and variables that indicate the likelihood of loan default among loan applicants. This objective includes:
1. Identifying Risky Applicants: Detecting individuals who are likely to default on their loans and taking appropriate actions, such as denying loans, adjusting loan amounts, or offering loans at higher interest rates to mitigate potential losses.
2. Minimizing Credit Loss: Minimizing the financial losses associated with borrowers who default on loans, known as credit loss. By identifying defaulters, the company can take proactive measures to reduce credit loss.
3. Enhancing Risk Assessment: Utilizing data-driven insights to understand the key factors influencing loan defaults, which can improve portfolio management and risk assessment processes.


### Dataset
[loan.csv](loan.csv) contains the complete loan data for all loans issued through the time period 2007 t0 2011. 

[Data_Dictionary.xlsx](Data_Dictionary.xlsx) describes the meaning of these variables

There are two types of decisions that could be taken by the company:

1. Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

    * Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

    * Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

    * Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

2. Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)


## Technologies Used
- seaborn - 0.13.0
- matplotlib - 3.8.1
- pandas - 2.1.2
- missingno - 0.5.2
- numpy - 1.26.1


## Analysis Approach
1. Data Overview
2. Data cleaning
3. Univatiate Analysis
4. Bivatiate Analysis
5. Time analysis

## Conclusions
- The majority of customers fall into high grade and Charge-Offs are more in lower grade segment.
- Many loans have debt consolidation purposes so they have many charge-off customers. Be careful with small business purposes, have a high charge-off ratio
- Home Ownership as own have less loans than mortgage and rent but the charge of ratio is similar. That’s mean borrowers who are classified as 'Renters' or have 'Mortgages' are more likely to experience loan defaults.
- The majority of customers have short-term loans, but long-term loans have a higher ratio of charged-off customers.
- A shorter employment length is associated with a higher level of risk
- The charge-offs are subject to higher interest rates and lower total payments

## Acknowledgements
- The project references insights and inferences from live presentation given by [Akashdeep Makkar](https://www.linkedin.com/in/akashdeep-makkar-12110880/) 
- You can find the data at- "loan.csv" within this repo.
- Refer Data dictionary- "Data_Dictionary.xlsx" for in depth understanding of the dataset.

## TODO
* Clean data for predict charge-off customer
* Predictive analyst 
## Contact
Created by [Huynh Viet Cuong](https://cuonghv0298.github.io/) - feel free to contact me by email vietcuong.ip@gmail.com!

