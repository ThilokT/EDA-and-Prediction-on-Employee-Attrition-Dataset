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

### 2. **Class Balancing**
- SMOTE was used to oversample the minority class (Attrition = Yes) in the training set.

### 3. **Evaluation Metrics**
- Accuracy, Precision, Recall, F1-Score, and Confusion Matrix were used to evaluate model performance.

---

##  Machine Learning Models and Results

The following classification models were trained and evaluated:

| Model                     | Accuracy |
|--------------------------|----------|
| Logistic Regression       | ~84.0%   |
| Decision Tree Classifier  | ~87.5%   |
| Random Forest Classifier  | ~88.9%   |
| XGBoost Classifier        | **~92.3%**   |

 **Best Model**: **XGBoost Classifier**  
XGBoost outperformed the other models with the highest accuracy and balanced performance across precision, recall, and F1-score.

---

