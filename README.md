# **LOAN-CREDIT-EDA-FINANCIAL-PREDICTIVE-ANALYTICS**
Risk analytics in banking and financial services in Real Business Scenario minimise the risk of losing money while lending to customers.

# Problem Statement:
To identify patterns which indicate if a client has difficulty paying their installments which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate

**Two types of risks are associated with the bank’s decision:**
- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company.
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.
 
# Problem Introduction:
- Predictive Analytics can be used to decide the credit worthiness of a customer and whether he/she can be issued a credit card or not.
- This assignment aims to give you an idea of applying **EDA in a real business scenario**. In this case study we are using **Exploratory Data Analytics** to do a case study on **"Loan's application"**. In this assignment, we will also develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.

# Business Objectives:
This case study aims to identify patterns which indicate if a client has difficulty paying their installments which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc. This will ensure that the consumers capable of repaying the loan are not rejected. 
**Identification of such applicants using EDA is the aim of this case study.**

In other words, the **Company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.**

To develop your understanding of the domain, you are advised to independently research a little about **risk analytics** - understanding the types of variables and their significance should be enough).

**When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:**

- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company.
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

The data given below contains the information about the loan application at the time of applying for the loan. It contains two types of scenarios:

1. **The client with payment difficulties**: `he/she had late payment more than X days on at least one of the first Y instalments of the loan in our sample,`
2. **All other cases** : `All other cases when the payment is paid on time.`

**When a client applies for a loan, there are four types of decisions that could be taken by the client/company:**
- **Approved**: The Company has approved loan Application.
- **Cancelled**: The client cancelled the application sometime during approval. Either the client changed her/his mind about the loan or in some cases due to a higher risk of the client he received worse pricing which he did not want.
- **Refused**: The company had rejected the loan (because the client does not meet their requirements etc.
- **Unused offer**: Loan has been cancelled by the client but on different stages of the process.

In this case study, we will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.

# DataSet Description:

 **This dataset has 3 files** as explained below: 

 1. **application_data.csv** contains all the information of the client at the time of application.
The data is about whether a **client has payment difficulties.**

2. **previous_application.csv** contains information about the client’s previous loan data. It contains the data whether the **previous application had been Approved, Cancelled, Refused or Unused offer.**

3. **columns_description.csv** is **data dictionary** which describes the meaning of the variables.

[Dataset Download Link](https://cdn.upgrad.com/UpGrad/temp/afe3690a-9d30-4f1d-b9ee-2d5d17881422/Dataset.txt)

# CONCLUSION WITH STRONG INDICATORS TO DRIVE BUSINESS DECISIONS
1. `Target/focused variable for "Current-Application" Dataset` - **TARGET**
2. `Target/focused variable for "Previous-Application" Dataset` - **NAME_CONTRACT_STATUS**

**Top Major variables to consider for loan prediction:**

- NAME_EDUCATION_TYPE         - AMT_INCOME_TOTAL               
- DAYS_BIRTH                  - AMT_CREDIT               
- DAYS_EMPLOYED               - AMT_ANNUITY             
- NAME_INCOME_TYPE            - CODE_GENDER                 
- NAME_HOUSING_TYPE                        

**To Minimize risk of loss, the above-mentioned variables should be evaluated before approving an application.**

### To whom should loan can be approved?

`1. Loan can approved of secondary education compare to higher education and lower education.`<br>
`2. Applicants having high income.`<br>
`3. Female applicants.`<br>
`4. Married applicant`<br>
1. Banks should focus more on contract type ‘Student’ ,’pensioner’ and ‘Businessman’ with housing type otherthan ‘Co-op apartment’ for successful payments.
2. Banks should focus less on income type ‘Working’ as they are having most number of unsuccessful payments.
3. Also with loan purpose ‘Repair’ is having higher number of unsuccessful payments on time.
4. Get as much as clients from housing type ‘With parents’ as they are having least number of unsuccessful payments.
5. Labourers, Sales Staff, Drivers, seems to be the most defaulters as we concluded earlier, further digging into the female candidates, most of the waiters, private service staff, realty agents, HR staff, IT Staff, Secretaries are the defaulters as compared to their counterparts.
6. Female applicants without car are the most defaulters.
7. Looking at the current and the previous data, Working, Commercial associates & State servants are mostly prone for being defaulters.
8. Most defaulters are in the low income range.

## Decisive Factor whether an applicant will be Repayer:
 - **NAME_EDUCATION_TYPE:** Academic degree has less defaults.
 - **NAME_INCOME_TYPE:** Student and Businessmen have no defaults.
 - **REGION_RATING_CLIENT:** RATING 1 is safer.
 - **ORGANIZATION_TYPE:** Clients with Trade Type 4 and 5 and Industry type 8 have defaulted less than 3% - 
 - **DAYS_BIRTH:** People above age of 50 have low probability of defaulting 
 - **DAYS_EMPLOYED:** Clients with 40+ year experience having less than 1% default rate
 - **AMT_INCOME_TOTAL:**Applicant with Income more than 700,000 are less likely to default
 - **NAME_CASH_LOAN_PURPOSE:** Loans bought for Hobby, Buying garage are being repayed mostly.
 - **CNT_CHILDREN:** People with zero to two children tend to repay the loans.

## Decisive Factor whether an applicant will be Defaulter:
- **CODE_GENDER**: Men are at relatively higher default rate
- **NAME_FAMILY_STATUS** : People who have civil marriage or who are single default a lot.
- **NAME_EDUCATION_TYPE** : People with Lower Secondary & Secondary education
- **NAME_INCOME_TYPE**: Clients who are either at Maternity leave OR Unemployed default a lot.
- **REGION_RATING_CLIENT** : People who live in Rating 3 has highest defaults.
- **OCCUPATION_TYPE** : Avoid Low-skill Laborers, Drivers and Waiters/barmen staff, Security staff, Laborers and Cooking staff as the default rate is high.
- **ORGANIZATION_TYPE** : Transport: type 3 (16%), Industry: type 13 (13.5%), Industry: type 8 (12.5%), and Restaurant: type 3 (16%) are the organisations with the greatest percentage of loans not repaid (less than 12 percent ). Because self-employed people have a high default rate, they should be avoided when applying for a loan or given a loan with a higher interest rate to reduce the chance of default.
- **DAYS_BIRTH** : Avoid young people who are in age group of 20-40 as they have higher probability of defaulting
- **DAYS_EMPLOYED**: People who have less than 5 years of employment have high default rate.
- **CNT_CHILDREN & CNT_FAM_MEMBERS**: Client who have children equal to or more than 9 default 100% and hence their applications are to be rejected.
- **AMT_GOODS_PRICE**: When the credit amount goes beyond 3M, there is an increase in defaulters.

# Acknowledgement:
This Assignment was part of Curriculum during EPGP-Data Science AI-ML (Business Analytics) from IIIT-B.

***@All Rights Reserved*** [Gurpreet Kaur Jethra](https://github.com/GURPREETKAURJETHRA)
