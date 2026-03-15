# Insurance Cost Analysis using Machine Learning

This project analyzes medical insurance costs and builds machine learning models to predict insurance charges based on demographic and health-related features.

The project demonstrates the complete data science workflow including data preprocessing, exploratory data analysis (EDA), model development, and model refinement using regression techniques.

---

## Dataset

Dataset Link: https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0101EN-Coursera/medical_insurance_dataset.csv

The dataset contains medical insurance information including:

- Age
- Gender
- BMI (Body Mass Index)
- Number of Children
- Smoking Status
- Region
- Insurance Charges

Source: IBM Developer Skills Network

---

## Project Workflow

### 1. Data Loading
The dataset was loaded using Pandas directly from an online source.

### 2. Data Cleaning
Data preprocessing steps included:

- Handling missing values
- Converting data types
- Replacing missing numerical values with mean
- Replacing missing categorical values with the most frequent value
- Rounding insurance charges to two decimal places

---

### 3. Exploratory Data Analysis (EDA)

Data visualization techniques were used to understand relationships between variables.

Visualizations included:

- Regression plot between **BMI and insurance charges**
- Box plot comparing **smokers vs non-smokers**
- Correlation heatmap to analyze relationships between variables

Key insight:
Smoking status shows a strong correlation with higher insurance charges.

---

### 4. Model Development

Several regression models were developed to predict insurance charges.

#### Linear Regression (Single Feature)

Predicting charges using only smoking status.

R² Score: **0.62**

---

#### Linear Regression (Multiple Features)

Using all available features:

- Age
- Gender
- BMI
- Number of children
- Smoker
- Region

R² Score: **0.75**

---

#### Pipeline Model

A machine learning pipeline was created using:

- StandardScaler
- PolynomialFeatures
- LinearRegression

R² Score: **0.84**

---

### 5. Model Refinement

Further improvements were made using Ridge Regression and Polynomial Features.

#### Ridge Regression

R² Score: **~0.72**

#### Polynomial + Ridge Regression

R² Score: **~0.81**

This improved the model’s ability to capture nonlinear relationships in the data.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Key Skills Demonstrated

- Data Cleaning and Preprocessing
- Exploratory Data Analysis
- Data Visualization
- Machine Learning Modeling
- Regression Analysis
- Feature Engineering
- Model Evaluation

---

## Project Structure
insurance-cost-analysis
│
├── insurance_analysis.ipynb
└── README.md

---

## Results

The project shows that:

- Smoking has the strongest influence on insurance charges
- Machine learning models can effectively predict insurance costs
- Feature engineering significantly improves model performance

Final Model R² Score: **~0.81**

---

## Author

Dhruvin Katrodiya

If you found this project useful, feel free to ⭐ the repository.
