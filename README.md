# creditscoring
Machine learning-based credit scoring models to predict the monthly default probability of credit card customers

# Overview
This project develops an end-to-end credit scoring and loss optimization tool for credit card default risk, designed to be accessible to both technical and non-technical users.

# Model selection
Three machine learning models were evaluated — XGBoost, Random Forest, and Neural Network — and benchmarked against each other using F1 score and recall on the default class. The Neural Network was selected as the best-performing model and used for all downstream analysis.

# Expected loss analysis
Using the default probabilities produced by the Neural Network, the project constructs a distribution of expected losses across the customer portfolio. Tail risk is then quantified at the 95th and 99th percentiles, and mitigation strategies are proposed and evaluated based on their effectiveness in reducing these concentrations.

# UI Tool 
The project is finalized as an interactive interface built with Streamlit, allowing non-technical users to query the default probability of individual customers within a few clicks. To launch the tool, run:
streamlit run UI_Tool.py
