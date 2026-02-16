# DonorsChoose-project-approval-analysis
This project analyzes DonorsChoose data to understand what factors influence whether a project is approved.

The goal is to apply a complete data science workflow, including:
- Business problem definition
- Data cleaning and preparation
- Exploratory Data Analysis (EDA)
- Predictive modeling
- Insight generation

This project was developed as part of a personal portfolio to demonstrate practical analytics and machine learning skills.

## Business Problem
Nonprofit crowdfunding platforms review thousands of project submissions. Not all submissions are approved.

This project explores:

**What factors influence project approval decisions?**

Understanding these drivers can help platforms:
- Improve submission quality
- Support new contributors
- Optimize review processes

## Dataset
Source: DonorsChoose dataset from Kaggle

The dataset contains project-level information, including:
- Teacher attributes
- Project categories
- Cost variables
- Preprocessed text fields
- Approval outcomes

**Note:** Due to file size constraints, the dataset is not included in this repository.
To reproduce the analysis, please download the dataset on Kaggle and place the csv file in a data folder.

## Data Preparation
Data cleaning steps included:
- Missing value handling
- Data type validation
- Business-rule validation
- Feature engineering

New features created:
- Total project cost
- Log-transformed cost variables
- Teacher experience signals
- Text length metrics

## Exploratory Data Analysis (EDA)
EDA focused on identifying patterns related to approval outcomes.

Key areas explored:
- Cost distributions
- Teacher experience effects
- Proposal richness indicators
- Category-level approval differences

## Modeling Approach
A Logistic Regression model was developed to predict project approval.

Why Logistic Regression:
- Suitable for binary classification
- Interpretable
- Strong baseline model

Challenge encountered:
- Class imbalance (many more approved projects)

Solution applied:
- Class weighting to improve minority class detection

## Model Performance
Baseline model:
- High accuracy
- Poor detection of not-approved projects

Balanced model:
- Lower accuracy (expected)
- Significant improvement in rejection detection

Key takeaway:
**Accuracy alone is not sufficient for evaluating imbalanced datasets.**

## Key Insights
The analysis suggests that approval decisions are influenced by:
- Total cost magnitude
- Teacher experience
- Proposal detail and richness
- Project category attributes

## Skills Demonstrated
This project demonstrates:
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Data cleaning & validation
- Feature engineering
- Exploratory Data Analysis
- Machine learning modeling
- Model evaluation & interpretation

## Limitations
- Dataset is preprocessed
- No donation outcome variables
- Text analysis limited to length-based features

## Future Improvements
Potential extensions:
- NLP-based text modeling
- Alternative ML models
- Threshold optimization

## Author
Dennis Ashiagbor
