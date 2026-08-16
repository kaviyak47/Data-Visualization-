# Stroke Prediction and Analysis
### Data Visualization Techniques Lab

This project analyzes the **Stroke Prediction Dataset** using Python-based data processing, exploratory data analysis (EDA), preprocessing techniques, statistical analysis, data visualization, and machine learning.

---

## Dataset

**Dataset:** Stroke Prediction Dataset
**Source:** [Kaggle — Stroke Prediction Dataset by fedesoriano](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

The dataset contains patient-related demographic, medical, and lifestyle information used to analyze and predict the occurrence of stroke. It contains **5,110 records and 12 columns**.

The dataset includes attributes such as:
- Gender
- Age
- Hypertension
- Heart Disease
- Ever Married
- Work Type
- Residence Type
- Average Glucose Level
- BMI
- Smoking Status
- Stroke

The `stroke` column is the target variable, where `1` represents a patient who had a stroke and `0` represents no stroke.

---

## Project Objective

The objective of this project is to analyze the Stroke Prediction dataset, perform data preprocessing, explore patient-related patterns, calculate statistical measures, apply data grouping and correlation analysis, and represent the results through suitable visualizations.

The project demonstrates how data analysis and visualization techniques can be used to understand:
- Stroke distribution
- Stroke patterns by gender
- Age-related patterns
- Average glucose-level variations
- BMI and other numerical relationships
- Patient characteristics across work types
- Correlations between numerical variables
- Distribution of stroke and non-stroke patients
- Relationships between health-related attributes

---

## Experiments

### Experiment 1 — Stroke Prediction Using Machine Learning

**Aim:**
To analyze the Stroke Prediction dataset using Exploratory Data Analysis (EDA), visualize important patient patterns, build a Logistic Regression model to predict stroke, evaluate the model, and export the processed data to Excel.

**Work Performed:**
- Dataset loading and inspection
- Dataset shape and information analysis
- Missing-value detection
- Missing BMI value handling
- Removal of the unnecessary ID column
- Stroke distribution visualization
- Stroke analysis by gender
- Stroke analysis by smoking status
- One-hot encoding of categorical variables
- Train-test splitting
- Logistic Regression model training
- Stroke prediction
- Accuracy calculation
- Confusion matrix generation
- Export of processed data to Excel

**Model:** Logistic Regression

**Outcome:**
A Logistic Regression model was trained to predict whether a patient is likely to have a stroke. The model was evaluated using accuracy and a confusion matrix.

---

### Experiment 2 — EDA – Data Cleaning

**Aim:**
To clean the Stroke Prediction dataset by detecting and handling missing values, removing duplicate and unnecessary data, checking data types, and normalizing numerical data.

**Work Performed:**
- Identification of missing values
- Handling missing BMI values using median replacement
- Duplicate-record detection
- Removal of duplicate records
- Removal of the `id` column
- Data-type inspection
- Min-Max Scaling
- Standardization using StandardScaler
- Display of the cleaned and normalized data

**Outcome:**
The dataset was successfully cleaned and numerical features were normalized using Min-Max Scaling and Standardization, preparing the dataset for further analysis.

---

### Experiment 3 — EDA – Data Inspection and Analysis

**Aim:**
To inspect and analyze the Stroke Prediction dataset using DataFrame operations, conditional filtering, descriptive statistics, and measures of central tendency and dispersion.

**Work Performed:**
- Viewing the first five records
- Viewing the last five records
- Inspecting dataset shape
- Inspecting column names
- Checking data types
- Filtering patients based on average glucose level
- Filtering patients based on age
- Selecting specific columns
- Calculating mean
- Calculating median
- Calculating mode
- Calculating range
- Calculating variance
- Calculating standard deviation
- Generating descriptive statistics

**Outcome:**
The experiment provides statistical insights into the numerical features of the Stroke Prediction dataset, particularly age and average glucose level.

---

### Experiment 4 — Data Visualization

**Aim:**
To visualize the Stroke Prediction dataset using Python by creating bar charts, pie charts, and line charts for better understanding of stroke patterns.

**Visualizations:**
- **Bar Chart:** Stroke cases by gender
- **Pie Chart:** Stroke and non-stroke distribution
- **Line Chart:** Average glucose level by age

**Outcome:**
The visualizations provide an intuitive understanding of stroke distribution, gender-wise stroke patterns, and changes in average glucose levels across different ages.

---

### Experiment 5 — Calculated Field and Data Visualization

**Aim:**
To analyze the Stroke Prediction dataset using Python by creating a calculated field and basic visualizations such as bar charts, line charts, and pie charts.

**Work Performed:**
A calculated field named **Patient Status** was created. The values are classified as:
- Stroke
- No Stroke

**Visualizations:**
- **Bar Chart:** Stroke cases by gender
- **Line Chart:** Average glucose level by age
- **Pie Chart:** Stroke and non-stroke patient distribution

**Outcome:**
The calculated field and visualizations provide a clearer understanding of patient stroke status and its relationship with gender and age-related glucose levels.

---

### Experiment 6 — EDA – Grouping and Aggregation

**Aim:**
To perform grouping and aggregation on the Stroke Prediction dataset using Pandas and analyze patient characteristics based on different categories.

**Work Performed:**
- Grouping patients based on gender
- Calculation of total patients by gender
- Calculation of average age by gender
- Calculation of average glucose level by gender
- Cross-tabulation of stroke cases by gender
- Grouping patients based on work type
- Calculation of total patients by work type
- Calculation of average age by work type
- Calculation of average glucose level by work type
- Bar-chart visualization of patients by gender

**Outcome:**
The grouping and aggregation analysis identifies differences in patient characteristics across gender and work-type categories.

---

### Experiment 7 — EDA – Correlation Analysis

**Aim:**
To analyze the relationship between numerical variables in the Stroke Prediction dataset using correlation analysis and a heatmap.

**Work Performed:**
The following numerical attributes were analyzed:
- Age
- Hypertension
- Heart Disease
- Average Glucose Level
- BMI
- Stroke

A correlation matrix was calculated and visualized using a heatmap.

**Visualization:** Correlation Heatmap

**Outcome:**
The correlation analysis provides an understanding of relationships between numerical features and helps identify variables that have stronger or weaker relationships with stroke.

---

## How This Project Aligns with Data Visualization

### 1. Comparison
Bar charts are used to compare:
- Stroke cases across genders
- Number of patients across categories
- Patient groups based on different attributes

### 2. Trends
Line charts are used to visualize:
- Average glucose level across different ages

### 3. Distribution
Pie charts are used to represent:
- Stroke vs non-stroke patients

### 4. Relationships
The project uses visualizations to study relationships such as:
- Age vs average glucose level
- Gender vs stroke
- Work type vs patient characteristics

### 5. Correlation
A correlation heatmap is used to show relationships between numerical variables such as:
- Age
- Hypertension
- Heart disease
- Average glucose level
- BMI
- Stroke

### 6. Statistical Analysis
Mean, median, mode, range, variance, standard deviation, and descriptive statistics are used to understand numerical data.

### 7. Multivariate Analysis
Multiple patient attributes are analyzed together to understand patterns associated with stroke occurrence.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab
- Excel
- GitHub

---

## Machine Learning

The project includes a basic machine-learning classification model.

**Algorithm Used:** Logistic Regression
**Target Variable:** `stroke`

Where:
- `0` → No Stroke
- `1` → Stroke

**Evaluation Metrics:**
- Accuracy
- Confusion Matrix

---

## Dataset Information

The original Kaggle dataset contains 5,110 records and 12 columns. The dataset provides demographic, medical, and lifestyle information for stroke prediction.

### Attributes

| Attribute | Description |
|---|---|
| id | Unique patient identifier |
| gender | Gender of the patient |
| age | Age of the patient |
| hypertension | Whether the patient has hypertension |
| heart_disease | Whether the patient has heart disease |
| ever_married | Whether the patient has ever been married |
| work_type | Type of work |
| Residence_type | Rural or Urban residence |
| avg_glucose_level | Average glucose level |
| bmi | Body Mass Index |
| smoking_status | Smoking status |
| stroke | Target variable indicating stroke occurrence |

*These attribute definitions follow the dataset's Kaggle documentation.*

---

## Project Structure

```
Stroke-Prediction-Analysis/
│
├── healthcare-dataset-stroke-data.csv
│
├── Experiment_1_Stroke_Prediction.ipynb
├── Experiment_2_Data_Cleaning.ipynb
├── Experiment_3_Data_Inspection.ipynb
├── Experiment_4_Data_Visualization.ipynb
├── Experiment_5_Calculated_Field.ipynb
├── Experiment_6_Grouping_Aggregation.ipynb
├── Experiment_7_Correlation_Analysis.ipynb
│
└── README.md
```

---

## Conclusion

The Stroke Prediction and Analysis project demonstrates a complete data-analysis workflow starting from data inspection and preprocessing to statistical analysis, visualization, correlation analysis, grouping, aggregation, and machine learning.

The project uses the Stroke Prediction dataset to demonstrate how different data analysis and visualization techniques can communicate information effectively. Through bar charts, line charts, pie charts, and correlation heatmaps, the project provides insights into stroke distribution, patient characteristics, glucose-level patterns, gender-wise differences, and relationships between numerical health attributes.

The combination of EDA, data preprocessing, statistical analysis, data visualization, grouping and aggregation, correlation analysis, and machine learning makes the project suitable for demonstrating the practical application of Data Visualization Techniques to a real-world healthcare dataset.

---

## Dataset Source

**Kaggle — Stroke Prediction Dataset**
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

The dataset documentation states that it is intended for predicting whether a patient is likely to experience a stroke based on demographic, disease, and lifestyle-related attributes.

---

## Repository

**GitHub Repository:**
https://github.com/kaviyak47/Data-Visualization-/edit/main/README.md

*Replace the above with your actual GitHub repository link after creating the repository.*
