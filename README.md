# Mobile Plan Recommendation Model

## 📊 Project Overview
This project develops a Machine Learning classification model to recommend the most suitable mobile plan (Smart or Ultra) for Megaline customers.
Using behavioral data from subscribers who have already migrated to the new plans, the model analyzes usage patterns to predict the optimal plan for users who are still on legacy plans.
The dataset was preprocessed beforehand, allowing this project to focus on model development, training, and evaluation.
The primary objective is to achieve the highest possible predictive accuracy, with a minimum required threshold of 0.75.

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
