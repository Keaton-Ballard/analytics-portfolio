# Welcome to My Portfolio!

I'm Keaton Ballard, a data analyst interested in automation, business operations, and data-driven decision-making. This portfolio showcases the scripts I created during my Data Analytics Master's and the custom code I wrote to improve HubSpot CRM workflows.


### Master's Program Data Analytics Projects

For my master's program, we could choose between 2 synthetic datasets we would work with throughout the program. The dataset I chose contained 10,000 rows of hospital patient data. Below are the several analyses I conducted on the dataset.

## [Project 1: Exploratory Analysis](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Exploratory_analysis.ipynb)

Conducted an initial deep-dive into patient readmission data using Chi-square tests, T-tests, and ANOVA. This analysis surfaced key features that showed statistically significant associations with readmission outcomes.

---

## [Project 2: Linear Regression Modeling](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Linear_regression.ipynb)

Built a linear regression model to quantify how variables like vitamin D levels, income, and age impacted patient charges. This project focused on predicting the TotalCharge variable while ensuring data quality and model interpretability.

---

## [Project 3: Logistic Regression Modeling](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Logistic_regression.ipynb)

Used logistic regression to classify patient readmission outcomes based on medical conditions. Evaluated how chronic illnesses and comorbidities influence the likelihood of readmission.

---

## [Project 4: Data Mining - Classification Method](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Data_mining_classification.ipynb)

Prepared and modeled patient data using classification techniques to predict readmission risk. Included feature engineering, categorical encoding, and data cleaning to support supervised learning.

---

## [Project 5: Data Mining - Prediction Method](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Data_mining_prediction.ipynb)

Developed a regression-based predictive model to estimate total patient charges. Emphasized data preprocessing, log transformation, and model evaluation using Random Forest Regressor.

---

## [Project 6: Data Mining - Clustering Method](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Data_mining_clustering_methods.ipynb)

Applied unsupervised clustering (K-Means) to segment patients based on demographics and billing data. The elbow method and silhouette score were used to determine the optimal cluster count.

---

## [Project 7: Data Mining - PCA Analysis](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Data_mining_PCA.ipynb)

Performed PCA to reduce dimensionality and reveal key components influencing variance in patient data. Included feature scaling, scree plot visualization, and interpretation of the loading matrix.

---

## [Project 8: Data Mining - Market Basket Analysis](https://github.com/Keaton-Ballard/analytics-portfolio/blob/main/Data_mining_market_basket_method.ipynb)

Conducted association rule mining on patient condition data using the Apriori algorithm. Transformed diagnosis data into a transactional format to discover frequently co-occurring conditions and risk factors.

---

### HubSpot Custom Code Projects 

(HubSpot scripts require a private app with the correct scopes and API key.) 

## [Project 9: Weighted HubSpot Lead Distributor](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/weighted-hubspot-lead-distributor)


This script automates the assignment of HubSpot contacts to owners (such as sales reps) using a **weighted random distribution** approach. Reps with more "weight" are more likely to be assigned a new contact.
Since using round-robin logic doesn't work well in HubSpot, this script enables a more customized and stable probability-based assignment strategy that efficiently distributes leads to reps with a simple syntax that simplifies changing the distribution weights.


---

## [Project 10: HubSpot Record Meeting Associatior](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-meeting-deal-associator)


Our sales process in HubSpot creates deal records after a contact book a meeting, which makes the meeting information only present in the contact record and not the deal record. This script corrects this error by automatically associating the most recently booked meeting with the most recent deal tied to a contact in HubSpot. Ensuring the sales reps have all the correct meeting and sales information in one place before they meet with their clients.


---

## [Project 11: HubSpot Phone Number Formatter](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-phone-number-formatter)


This script automates the formatting of U.S. phone numbers for contacts in HubSpot. It standardizes phone numbers into the format `(XXX) XXX-XXXX` using a Python script that I deploy in a HubSpot *custom code action* in workflow, ensuring that all phone numbers in our CRM will have the same format. It also includes built-in error handling, API rate limit retries, and permission checks to ensure it stays within HubSpot's API limits.

---

## [Project 12: Hubspot Smart Record Merger](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-smart-record-merger)


The purpose of this script is to automatically detect and merge a specialized group of duplicate HubSpot contacts. I created this automation because many contacts use one email on the ad form and a separate email on the meeting book form. HubSpot's merging system is currently manual. It first attempts to identify duplicates using the contact's phone number. It returns to searching by exact first and last name if no matches are found. The goal is to ensure that the correct records are being merged within the CRM.

<!-- force update -->


