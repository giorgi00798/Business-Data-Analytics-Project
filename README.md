# Data Analytics in Motorsport: Predicting Formula 1 Race Outcomes

This repository contains the work for my dissertation project, where I analyse historical Formula 1 data and build machine learning models to predict race outcomes.The focus is on understanding which factors matter the most during a race weekend and how well we can predict a driver's performance using real-world data.

The project has two main goals:
- Predict whether a driver finishes in the **Top 10**
- Predict the **exact finishing position**

Everything - from raw dataset inspection to feature engineering and final model evaluation - is included in the notebook.


## About the Dataset

The project is based on the **Formula 1 World Championship (1950-2024)** dataset from Kaggle.
Since the dataset is stored across many different tables, I grouped them into categories dependingon how important they are for building a race-level dataset.

### **Key Tables**
These tables describe the actual race results and are essencial for modelling:
- `results` - final race outcome (positions, points, laps, etc.)
- `races` - race information (year, round, circuit)
- `drivers` - driver details (name, nationality, DOB)
- `constructors` - team information
- `circuits` - track details (location, altitude)

### **Supporting Tables**
These add more context and help generate useful features:
- `qualifying`
- `sprint_results`
- `pit_stops`
- `driver_standings`
- `constructor_standings`
- `constructor_results`
- `lap_times`
- `status`
- `seasons`

Before merging, all tables were checked for missing values, duplicated rows and incorrect data types.
The cleaned tables were then merged into a **single race-level driver dataset**, which is the foundation of all modelling.


### What the Notebook Includes

The notebook contaions the entire workflow of the project:

### **1. Data Presentation**
- loading all tables
- reviewing each one
- handling duplicates
- converting data types
- fixing missing values
- merging everything into one modelling dataset
- creating two new features:
  - `driver_experience`
  - `recent_form_3`

### **2. Exploratory Data Analysis (EDA)**
I explored:
- how qualifying affects race results
- the impact of pit stop strategy
- constructor dominance across decades
- driver career points
- correlations between key race features

These findings helped shape the modelling approach.

### **3. Baselina Models**
Two simple models were used to establish a baseline:
- Logistic Regression for Top 10 classification
- Linear Regression for exact finishing position

### **4. Advanced Models**
I them built more sophisticated models, including:
- Random Forest Classifier / Regressor
- Gradient Boosting Classifier / Regressor

Gradient Boosting performed the best in both tasks.

### **5. Model Evaluation**
The notebook includes:
- accuracy, precision recall, F1
- RMSE, MAE, R2
- confusion metrics
- resitual analysis
- ROC curve
- feature importance
- SHAP value explanations

This helps interpret model behavior and understand which features matter most.

## Files in This Repository
- **Data_Analytics_in_Motorsport_Predicting_Formula_1_Race_Outcomes.ipynb** - full code and model development
- **Dissertation.pdf** - written dissertation connected to this analysis
