# Employee Attrition: EDA and Prediction

##  Project Purpose

The purpose of this project is to explore and analyze employee attrition data and develop a predictive model that can identify the likelihood of an employee leaving a company. The insights gained from the exploratory data analysis (EDA) help HR teams understand patterns and factors contributing to attrition, and the predictive model can serve as an early warning system to aid in employee retention strategies.

---

## 🛠️ Tools and Libraries Used

This project is implemented in a Jupyter Notebook using Python and the following libraries:

- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning and preprocessing
- **XGBoost**: Gradient boosting algorithm for classification
- **Imbalanced-learn (SMOTE)**: Oversampling technique to balance classes

---

## 📊 Data Analysis and Preprocessing

### 1. **Data Loading and Overview**
- The dataset was loaded using Pandas.
- Initial exploration included checking for missing values, understanding data types, and getting descriptive statistics.

### 2. **Exploratory Data Analysis (EDA)**
- Visualizations were used to understand the distribution of features like:
  - Age, Gender, Education, Job Role, Department
  - Job Satisfaction, Monthly Income, Work-life Balance, etc.
- Correlation analysis was performed to identify relationships between variables.

### 3. **Data Cleaning and Feature Engineering**
- Unnecessary columns (e.g., Employee ID) were dropped.
- Categorical variables were encoded using one-hot encoding.
- Numerical features were scaled using `StandardScaler`.

### 4. **Handling Class Imbalance**
- The dataset showed imbalance between "Yes" and "No" in the attrition column.
- SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the classes before training.

---

## Model Training and Evaluation

### 1. **Model Selection**
- An XGBoost Classifier was chosen for its efficiency and performance on classification tasks.

### 2. **Training Process**
- Data was split into training and testing sets (typically 80/20 split).
- SMOTE was applied to the training data.
- The model was trained using the balanced dataset.

### 3. **Evaluation Metrics**
- Accuracy, Precision, Recall, F1-Score, and Confusion Matrix were used to evaluate model performance.
- The results demonstrated the model's ability to accurately predict employee attrition.


