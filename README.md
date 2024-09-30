# Home-Credit-Scorecard-Model
Final Task: Project Based Internship Home Credit Indonesia x Rakamin Academy

## Project Background

Home Credit Indonesia is dedicated to enhancing its credit scoring system, ensuring that deserving customers have access to the loans they need. Currently, the company employs various statistical methods and Machine Learning techniques to predict credit scores. Despite these efforts, there is still considerable untapped potential within the available data. By optimizing data utilization, Home Credit aims to create a more accurate and fair assessment process, reducing the likelihood of capable borrowers being unjustly denied loans.

This project focuses on developing an improved credit scorecard model that not only evaluates customer creditworthiness effectively but also tailors loan structures to promote successful repayments. With the right approach, Home Credit can better serve its customers while mitigating risk.

## Problem

Home Credit faces challenges in accurately assessing credit risk, leading to the rejection of customers who are financially capable of repaying loans. Current models may not fully capture all relevant factors, resulting in missed opportunities for lending and potential customer dissatisfaction.

## Goals

Develop a more precise credit scoring model using Machine Learning techniques, create a reliable scorecard that improves loan performance, enhances customer satisfaction, and supports responsible lending practices.

## Data understanding
- The dataset provided consists of 307.511 entries and 122 columns
- The dataset consists of 106  numeric columns and 16 categorical columns
- There are 67 columns with missing (null) data in the dataset
- No duplicate data
- Features with more than 40% missing data are removed to avoid unreliable imputation, reduce bias, and improve model performance by maintaining data quality and simplicity.
- To handle anomalous values we replaced the value with the mode to maintain data consistency.
- Outliers are removed by calculating the Z-scores of the data and filtering out values that are more than 3 standard deviations away from the mean.


## Insight Data

![image](https://github.com/user-attachments/assets/2dee44f5-c655-42a2-8aad-13dfa3c89aa1)

Based on the pict, 92% of customers managed to repay their loans on time, while 8% encountered difficulties. This notable discrepancy leads us to investigate the factors that set these two groups apart, specifically the characteristics that contribute to timely loan repayment.

![image](https://github.com/user-attachments/assets/6c4f938a-aec0-4add-b34d-75746d1f643b)

- Married individuals show a higher rate of successful loan repayment (68%) compared to unmarried individuals (24%).
- Meanwhile, the proportion of constrained (defaulting or struggling) customers is relatively low, with married individuals at 6% and unmarried individuals at only 2%.
- This suggests that being married may be associated with more reliable loan repayment behavior.

![image](https://github.com/user-attachments/assets/26625ff8-b55a-4106-9f12-11f75eaa4130)

- 92% of the adult category falls under the Unconstrained group, indicating that they successfully repay their loans on time.
- 94% of older customers are categorized as Unconstrained, highlighting their reliability in loan repayment.
- Although 89% of young adults are in the Unconstrained group, 11% experience repayment issues. This suggests a need for additional support or financial education for this age group.

![image](https://github.com/user-attachments/assets/68e1f7e8-4bd1-4b95-9f32-a2343c667c25)

Clients with Maternity leave and Unemployed income types have the highest risk of repayment issues, with TARGET percentages of 40% and 36%, indicating they struggle the most with timely loan repayments compared to other income types.

![image](https://github.com/user-attachments/assets/89cc34b8-3eb6-4168-96cc-883dc3862dff)

There is no significant difference in the contract type regarding repayment issues. While Cash Loans are the preferred choice among customers, the percentage of repayment problems is similar for both cash loans and revolving loans.

![image](https://github.com/user-attachments/assets/1e02ddd8-dfba-4ea2-8188-74437ae4b9fa)

- Occupations such as Accountants, Core Staff, IT Staff, High-skill tech staff, HR Staff, and Managers show a high percentage of Unconstrained customers (94% or above), meaning most individuals in these roles do not face issues repaying loans.
- Laborers, Drivers, Sales staff, and Cleaning staff have a relatively higher proportion of Constrained customers, ranging from 10% to 11%. Notably, Low-skill laborers show a Constrained rate of 17%, indicating financial instability.
- Recommendation: Lenders could consider stricter credit evaluations and tailored financial products for high-risk occupations such as laborers and drivers, as well as providing targeted financial education.

## Data Preparation

![image](https://github.com/user-attachments/assets/bbcb4103-30f1-40c9-8f0c-0f1bbe1c6324)

## Modeling

![image](https://github.com/user-attachments/assets/cfc38f10-30ea-4784-aea4-4ee6c21a5dd7)

Random Forest (Oversampling) as the best model because it has the highest testing accuracy of 0.96 and a good balance in precision, recall, and f1-score, all at 0.96.

## Summary

- The Home Credit Scorecard Model analysis identifies key customer segments for revolving loan contracts, focusing on individuals with income types such as business owners, maternity leave recipients, students, and unemployed individuals to tailor effective loan offerings.
- Recommendations include launching campaigns targeting accountants, the largest customer group with the best loan repayment rates, as well as creating targeted advertisements for HR professionals, IT specialists, and real estate agents to boost loan applications.
- Following a thorough evaluation, the Random Forest machine learning model is selected as the primary tool for predicting customer loan payment issues. This model demonstrates robust performance in identifying potential risks, enabling proactive management of possible loan defaults.

