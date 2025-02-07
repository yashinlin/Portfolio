
# Project Title: Prediction of past due loans in Home Credit Group

# Context
The [Home Credit Group](https://en.wikipedia.org/wiki/Home_Credit) operates in nine countries and focuses on installment lending primarily to people with little or no credit history. Loans can be obtained through retail shops, online through Home Credit's marketplaces in Russia, China, Philippines and Vietnam, and at third-party online stores using an app. 

The objective for this project is to predict which loans provided by Home Credit Group will be past due (ie. including both late payments and defaults).

# Summary of Findings
* Final model 

### Usage Instructions
* * Project code housed in Jupyter notebooks in the following order:
  01 Application_train data cleaning + EDA.ipynb
  02 Application_train modelling.ipynb
  03 Modelling using features from other tables.ipynb
* Each notebook starts with a high level summary of the key findings for the corresponding notebook 

### Key File Names
* Notebook files: 
    01 Risk_eval data cleaning + EDA.ipynb  
    02 Risk_eval modelling.ipynb  
    03 Features from other tables.ipynb  
* Python libraries (numbers correspond to notebooks): ./utils/libraries01 and libraries02_03
* Functions: ./utils/functions.py

### Final Model

The final model included 29 features. The top ones, in reverse order of importance, were:
* _Two features for normalized scores from an external data source not further identified in data dictionary_
* Kind of goods the client applied for in the previous application
* Client age in days
* Loan annuity
* Registration age in days
* Number of days before the application the client changed their identity document with which he applied for the loan
* Number of days since last phone change
* Credit-to-income ratio
* Normalized population of region where client lives (higher number means the client lives in more populated region)
* Annuity-to-income-ratio
* Total number of days installments paid early
* Average number of days installments paid early
* Proportion of late payments
* Number of days before the application the person started current employment
* Number of installment payments
* Number of days since last ID change
* Income
* Approximate hour the client applied
* Number of previous applications


