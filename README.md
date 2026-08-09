# Mobile Plan Recommendation Model

## 📊 Project Overview
This project develops a Machine Learning classification model to recommend the most suitable mobile plan (Smart or Ultra) for Megaline customers.
Using behavioral data from subscribers who have already migrated to the new plans, the model analyzes usage patterns to predict the optimal plan for users who are still on legacy plans.
The dataset was preprocessed beforehand, allowing this project to focus on model development, training, and evaluation.
The primary objective is to achieve the highest possible predictive accuracy, with a minimum required threshold of 0.75.

## 💼 Business Problem

Megaline is transitioning customers from its legacy mobile plans to two newer plans: Smart and Ultra. However, customers have different communication and data-consumption patterns, making it difficult to determine which plan is most appropriate for each subscriber.

Without a data-driven recommendation approach, plan upgrades may rely on broad customer segments or manual assumptions, which can result in customers being assigned to plans that do not match their actual usage.

The business needs to answer questions such as:
- Which mobile plan is most suitable for each customer?
- What usage patterns differentiate Smart customers from Ultra customers?
- Can a customer's calling, messaging, and internet usage predict the plan they are most likely to need?
- Which legacy-plan customers are likely to benefit from migrating to Smart or Ultra?
- How accurately can customer behavior be used to automate plan recommendations?
- Can Megaline improve customer targeting while reducing the need for manual plan recommendations?

Without a predictive solution, Megaline risks recommending plans that do not align with customer usage, potentially affecting customer satisfaction, retention, and revenue opportunities.

## ⚙️ Skills Developed

#### 🛠️ Tools

`Python` `Pandas` `NumPy` `Scikit-learn` `Jupyter` `Matplotlib` `Git` `GitHub`

#### Data Analysis & Preparation
- Exploratory Data Analysis (EDA)
- Behavioral Data Analysis
- Data Cleaning & Validation
- Feature Analysis
- Data Preparation for Machine Learning
- Train / Validation / Test Data Splitting

#### Machine Learning
- Supervised Learning
- Binary Classification
- Decision Tree Classifier
- Random Forest Classifier
- Logistic Regression
- Model Training
- Model Prediction

#### Model Development
- Feature Selection
- Hyperparameter Tuning
- Model Configuration
- Model Training & Validation
- Algorithm Comparison
- Model Performance Optimization

#### Model Evaluation
- Accuracy Score
- Validation Performance Analysis
- Test Set Evaluation
- Model Comparison
- Performance Benchmarking
- Model Selection
- Minimum Performance Threshold Validation

#### Predictive Analytics
- Customer Behavior Prediction
- Mobile Plan Recommendation
- Usage Pattern Analysis
- Customer Segmentation by Behavior
- Predictive Modeling
- Automated Plan Recommendation

#### Business Analytics
- Business Problem Translation
- Customer Targeting
- Plan Recommendation Strategy
- Data-Driven Decision Making
- Customer Usage Analysis
- Predictive Decision Support
- Business-Oriented Model Selection

## 📊 Dataset Description
The dataset contains behavioral data from Megaline subscribers, including:
- Number of calls
- Total call duration
- Internet usage (MB)
- Number of text messages
- Current mobile plan (target variable)

The target variable is binary:
- Smart
- Ultra

## ⚙️ Methodology
The project follows a structured Machine Learning workflow:
1. Model Development
- Three classification models were trained:
    - Decision Tree Classifier
    - Random Forest Classifier
    - Logistic Regression

2. Data Splitting
- Train / Validation / Test split
- Hyperparameters

3. Model Evaluation
- Performance metric: Accuracy
- Minimum required accuracy: 0.75
- Comparison of model performance to select the best-performing algorithm

## 📈 Results
- Three classification models were evaluated:
    - Random Forest
        - Accuracy: 0.797264
        - Best overall performance
        - Highest predictive capability
    - Decision Tree
        - Best depth: 3
        - Validation Accuracy: 0.78855721
        - Strong performance with controlled complexity
    - Logistic Regression
        - Accuracy: 0.75373
        - Lowest performance among the three models
        - Still exceeded the required threshold

- Conclusion <br>
    - All three models surpassed the required accuracy threshold of 0.75.However, the Random Forest Classifier achieved the highest accuracy and demonstrated superior predictive performance. Therefore, Random Forest is recommended as the optimal model for Megaline to accurately predict the most suitable plan for each customer, supporting data-driven decision-making and improving customer targeting.

## ▶️ How to Run the Project
1.	Clone this repository: git clone https://github.com/alangudi417/mobile-plan-model-recommendation.git  
2.	Navigate to the project folder: cd mobile-plan-model-recommendation
3.	Create and activate virtual environment: python -m venv venv venv\Scripts\activate # Windows source venv/bin/activate # Mac/Linux
4.	Install dependencies: pip install -r requirements.txt
5.	Launch Jupyter Notebook: jupyter notebook
6.  Open notebooks/mobile_plan_model.ipynb
