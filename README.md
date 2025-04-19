# Employee Attrition: EDA and Prediction

##  Project Purpose

The purpose of this project is to explore and analyze employee attrition data and develop a predictive model that can identify the likelihood of an employee leaving a company. The insights gained from the exploratory data analysis (EDA) help HR teams understand patterns and factors contributing to attrition, and the predictive model can serve as an early warning system to aid in employee retention strategies.

---

##  Tools and Libraries Used

This project is implemented in a Jupyter Notebook using Python and the following libraries:

- **Pandas**: Data manipulation and analysis  
- **NumPy**: Numerical operations  
- **Matplotlib & Seaborn**: Data visualization  
- **Scikit-learn**: Machine learning and preprocessing  
- **XGBoost**: Gradient boosting algorithm for classification  
- **Imbalanced-learn (SMOTE)**: Oversampling technique to balance classes  

---

##  Data Analysis and Preprocessing

### 1. **Data Loading and Overview**
- The dataset was loaded using Pandas.
- Initial exploration included checking for missing values, understanding data types, and getting descriptive statistics.

### 2. **Data Cleaning and Feature Engineering**
- Unnecessary columns (e.g., Employee ID) were dropped.
- Categorical variables were encoded using one-hot encoding.
- Numerical features were scaled using `StandardScaler`.
  
### 3. **Exploratory Data Analysis (EDA)**
- Visualizations were used to understand the distribution of features like:
  - Age, Gender, Education, Job Role, Department
  - Job Satisfaction, Monthly Income, Work-life Balance, etc.
- Correlation analysis was performed to identify relationships between variables.

### 4. **Handling Class Imbalance**
- The dataset showed imbalance between "Yes" and "No" in the attrition column.
- SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the classes before training.

---

##  Model Training and Evaluation

### 1. **Train-Test Split**
- The dataset was split into 80% training and 20% testing sets.

.

### 3. **Evaluation Metrics**
- Accuracy, Precision, Recall, F1-Score, and Confusion Matrix were used to evaluate model performance.

---

##  Machine Learning Models and Results

The following classification models were trained and evaluated using balanced training data (via SMOTE) and standardized features. Below are the models ranked by accuracy:

| Model                     | Accuracy Score (%) |
|--------------------------|--------------------|
| LightGBM                 | **75.85**          |
| Gradient Boosting        | 75.59              |
| Ada Boost                | 75.32              |
| XGBoost                  | 75.23              |
| Random Forest            | 74.64              |
| Extra Trees              | 74.34              |
| Support Vector Classifier (SVC) | 73.44        |
| Logistic Regression       | 71.78              |

 **Best Performing Model**: **LightGBM**

LightGBM had the highest accuracy at **75.85%**. Though closely followed by Gradient Boosting and Ada Boost, LightGBM demonstrated a slight edge in performance. 

