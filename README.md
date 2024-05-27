# Project-Reducing_Loan_Investment_Risk
Kaggle Lending Club dataset can be found at: 
https://www.kaggle.com/datasets/wordsforthewise/lending-club

## Table of Contents

- [Project Overview](#project-overview)
- [Business Understanding](#business-understanding)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)

## Project Overview

This project focuses on LendingClub, a peer-to-peer lending company based in the United States with its headquarters in San Francisco, California. LendingClub made history by becoming the first peer-to-peer lender to register its loan offerings as securities with the Securities and Exchange Commission (SEC) and by providing loan trading on a secondary market. It has earned the distinction of being the world's largest peer-to-peer lending platform.

## Business Understanding

You are a part of the LendingClub team, a company that specializes in providing a variety of loans to urban customers. When the company receives a loan application, it faces a critical decision-making process regarding loan approval based on the applicant's profile. This decision process carries two significant risks:

### Risk of Loan Repayment

If the applicant is likely to repay the loan, not approving the loan results in a loss of potential business for the company.

### Risk of Loan Default

If the applicant is not likely to repay the loan and is at risk of defaulting, approving the loan may lead to financial losses for the company.

The provided dataset contains information about past loan applicants and whether they 'defaulted' or not. The primary objective is to identify patterns and indicators that can predict if a person is likely to default. This knowledge enables the company to take actions such as denying the loan, reducing the loan amount, or offering loans to risky applicants at higher interest rates, among other strategies.

When a person applies for a loan, two types of decisions can be made by the company:

### Loan Accepted

If the company approves the loan, there are three possible scenarios:

- **Fully Paid:** The applicant has fully paid the loan, including the principal and interest.
- **Charged-Off:** The applicant has not paid the installments on time for an extended period, indicating loan default.

### Loan Rejected

In cases where the company rejects the loan (often due to the applicant not meeting their requirements), no transactional history with the company is available. Therefore, data for rejected applicants is not present in this dataset.

## Business Objectives

LendingClub, as the largest online loan marketplace, offers personal loans, business loans, and financing for medical procedures, providing the advantage of lower interest rates through a fast online interface.

One of the most significant sources of financial loss for lending companies is granting loans to "risky" applicants, resulting in credit loss. Credit loss represents the amount of money lost by the lender when borrowers fail to pay back the borrowed amount, effectively defaulting on their loans. In this context, customers labeled as 'charged-off' are considered 'defaulters.'

The key business objective of this case study is to identify and understand the factors driving loan defaults. This includes identifying variables that strongly indicate the likelihood of default. By achieving this objective, the company can use this knowledge to assess and manage the risk within its portfolio.

In essence, LendingClub aims to identify risky loan applicants, reduce such loans, and minimize credit losses. The identification of these applicants using EDA and machine learning is the core focus of this case study.

To enhance your domain understanding, it's advisable to conduct independent research on risk analytics, including an understanding of the types of variables and their significance in the context of risk assessment and mitigation.


## Exploratory Data Analysis (EDA)

In the EDA process, you explored the dataset, examining the relationships between columns based on the 'loan_status' and visualized these relationships using graphs. You may have used tools like Matplotlib, Seaborn, or other data visualization libraries to create these graphs. Here's a summary:

- **Data Exploration:** You began by understanding the dataset's structure, including the meaning and types of each column. This phase helped you to grasp the data's context and the initial challenges.

- **Data Visualization:** You created various graphs to visualize relationships between columns based on 'loan_status.' These graphs could include bar plots, scatter plots, or any other relevant visualization methods that help identify patterns or trends.

## Data Preprocessing

In the data preprocessing stage, you prepared the dataset for modeling by addressing issues like missing values, duplicate entries, and converting data types where necessary. This phase is crucial for ensuring that the dataset is clean and suitable for training machine learning models. Here's what you did:

- **Handling Missing Values:** You identified and handled missing values in the dataset. Common techniques include imputation, removal of rows or columns, or using domain knowledge to fill in missing data.

- **Dealing with Duplicate Entries:** You identified and addressed duplicate entries, if any, to prevent them from skewing the analysis or modeling results.

- **Data Type Transformation:** Some machine learning algorithms require specific data types for input features. You converted data types to match model requirements, such as converting categorical data to numerical format.

## Modeling

In the modeling phase, you selected and trained machine learning models to predict 'loan_status.' You utilized popular libraries like XGBoost, CatBoost, and Random Forest for this task. The process typically involves the following steps:

- **Data Split:** You divided the dataset into training and testing sets to assess model performance accurately.

- **Model Selection:** You chose appropriate machine learning models for classification tasks. In your case, you used XGBoost, CatBoost, and Random Forest classifiers.

- **Model Training:** You trained the selected models using the training data, allowing them to learn patterns and relationships within the data.

- **Model Evaluation:** You evaluated model performance using appropriate metrics, which might include accuracy, precision, recall, F1-score, and AUC-ROC, depending on your specific business goals.

- **Hyperparameter Tuning:** You may have performed hyperparameter tuning to optimize model performance, using techniques like grid search or random search.

- **Predictions:** After the models were trained and tuned, you used them to make predictions on the testing data.

- **Model Performance Assessment:** You assessed the model's accuracy, or other relevant metrics, to determine how well it can predict 'loan_status.' This step helps in selecting the best-performing model for your business objectives.

The successful completion of these stages would have allowed you to gain insights into the relationships within the data, prepare it for machine learning, and select the most suitable model to predict loan outcomes effectively. This is a common pipeline in data science projects, ensuring the data is processed correctly and the models are well-tuned for optimal performance.
