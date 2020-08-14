# Bank-Marketing-Analysis
Find the best strategies to improve for the next marketing campaign. How can the financial institution have a greater effectiveness for future marketing campaigns? In order to answer this, we have to analyze the last marketing campaign the bank performed and identify the patterns that will help us find conclusions in order to develop future strategies.
The three main questions answered in this project are:
Question 1: Is the account balance related to education level?
Question 2: What make your customer default?
Question 3: How to acquire more deposits for your bank?
### Summary of the results (takeaways)
1. Pay attention to customers who engaged in the last campaign and made a deposit. We usually will guess that those customers will not make deposits in the consecutive campaigns. But we are wrong. Those customers will be high likely to participate in your new campaign.
2. Try to make customers more engaged during the contact. Banks should do more research about the customer before the contact. If you make your customer willing to talk with your more than 8 minutes, you may get a new deposit.
3. Choose a right time to conduct the campaign. The project result shows us it’s better to start a campaign in March or October. Only 10%-20% customers will say no to you during these months.
Find more details from this [Medium article](https://medium.com/@JinzeL/know-your-customers-and-get-more-deposits-for-your-bank-60c3f4036398)
## Installation
This project runs in python 3.7. You need to install several python library to run this project, including:
1. numpy
2. pandas
3. matplotlib
4. seaborn
5. sklearn
6. xgboost
## Files Description
- data folder: contains all data files
- references folder: contains all references (data attributes dictionary)
- Bank Marketing Analysis.ipynb: Jupyter Notebook shows all codes and analytics
- LICENSE: license used for this repo

## Attributes Description
### Input variables
#### bank client data:
1. age: (numeric)
2. job: type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
3. marital: marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
4. education: (categorical: primary, secondary, tertiary and unknown)
5. default: has credit in default? (categorical: 'no','yes','unknown')
6. housing: has housing loan? (categorical: 'no','yes','unknown')
7. loan: has personal loan? (categorical: 'no','yes','unknown')
8. balance: Balance of the individual.

#### Related with the last contact of the current campaign:
8. contact: contact communication type (categorical: 'cellular','telephone')
9. month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
10. day: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
11. duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

#### other attributes:
12. campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
13. pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
14. previous: number of contacts performed before this campaign and for this client (numeric)
15. poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

### Output variable (desired target)
21. deposit: has the client subscribed a term deposit? (binary: 'yes','no')

## Reference
1. [Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014
2. Bank Marketing Dataset - [from Kaggle](https://www.kaggle.com/janiobachmann/bank-marketing-dataset)
3. Bank Marketing Campaign || Opening a Term Deposit, [Kaggle Kernel by Janio Martinez](https://www.kaggle.com/aleksandradeis/bank-marketing-analysis#Introduction)
4. Bank Marketing Analysis, [Kaggle Kernel by Aleksandra Deis](https://www.kaggle.com/aleksandradeis/bank-marketing-analysis/notebook)