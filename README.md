# Startup Prediction  

The goal of this project is to build a machine learning model that predicts whether a startup will succeed or fail based on various features. This is a **binary classification problem** involving both numerical and categorical data. By analyzing the dataset and training models, the project aims to provide insights that can guide investors and stakeholders in making data-driven decisions.  

---

## Objectives  

### 1. Data Understanding and Preprocessing  
- Import and organize libraries for analysis and modeling.  
- Load and explore the dataset.  
- Identify and handle missing values.  
- Analyze numerical and categorical features.  
- Perform feature engineering and selection.  
- Identify and handle outliers.  

### 2. Feature Engineering and Selection  
- Assess feature importance.  
- Create new features where relevant.  
- Remove redundant or highly correlated variables.  

### 3. Model Building and Evaluation  
- Train multiple classification models.  
- Validate and evaluate model performance using accuracy, precision, recall, F1-score, and ROC-AUC.  
- Compare models to select the most effective one.  

### 4. Deployment and Insights  
- Interpret results from the final model.  
- Highlight the most impactful features influencing startup success.  

---

## Data Preprocessing  

### Handling Missing Values  
The dataset contains missing data in multiple columns, such as company age, internet activity score, employee count, funding details, and education specialization.  
- Columns with excessive missing values were dropped.  
- Critical columns were imputed with mean, median, or mode, depending on the variable type.  

### Handling Correlated and Redundant Variables  
- Strongly correlated features were removed to reduce multicollinearity.  
- Features directly dependent on the target variable were excluded to avoid data leakage.  

---

## Exploratory Data Analysis  

Key observations from feature analysis include:  
- Younger startups (0 years old) dominate both successful and failed categories.  
- Companies with stable employee counts tend to perform better.  
- Certain industries and geographic locations show stronger success patterns.  
- Internet activity score and industry trends show measurable influence on outcomes.  

---

## Models Implemented  

The following machine learning models were trained and compared:  

1. **Logistic Regression** – simple and interpretable baseline.  
2. **Decision Tree Classifier** – captures non-linear patterns.  
3. **Random Forest Classifier** – reduces overfitting using ensembles.  
4. **XGBoost** – efficient gradient boosting with high performance.  
5. **Gaussian Naive Bayes** – assumes Gaussian distribution of features.  
6. **Bernoulli Naive Bayes** – works well with binary features.  

---

## Model Comparison  

Evaluation metrics used:  
- **Accuracy** – overall correctness of predictions.  
- **Precision** – proportion of correctly predicted positives.  
- **Recall** – proportion of actual positives correctly identified.  
- **F1-score** – balance between precision and recall.  
- **ROC-AUC** – ability to distinguish between classes.  

### Results  
- Logistic Regression provided strong baseline performance.  
- XGBoost showed the highest accuracy and robustness.  
- Ensemble models generally outperformed single classifiers.  

---

## Feature Importance  

Using XGBoost’s feature importance:  
- **Focus functions of company operation** and **highest education level** were the strongest predictors of success.  
- Funding- and investor-related features were less reliable due to missing or inconsistent data.  

---

## Final Model  

- **Best Model:** XGBoost with feature selection.  
- **Performance:**  
  - Accuracy: ~91%  
  - Precision: 0.91  
  - Recall: 0.89  
  - F1-score: 0.90  
- Balanced performance across both classes with minimal bias.  

---

## Conclusion  

The project successfully built a predictive model for startup success.  

Key takeaways:  
- Data preprocessing and feature selection significantly improved model stability.  
- Logistic Regression provided interpretability, while XGBoost provided superior accuracy.  
- The model can assist in evaluating startup viability, supporting informed decision-making for investors and stakeholders.  

