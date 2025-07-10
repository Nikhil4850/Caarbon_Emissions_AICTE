# Caarbon_Emissions_AICTE

**This is the project about CO2 Emission Prediction**

### 🌍 Carbon Emission Prediction using Machine Learning


# WEEK 1 : Understanding the Problem & Dataset
**Prediction of CO2 emissions from country-specific data**
### 🧠 Objective:
To understand the environmental issue of rising CO₂ emissions and explore how machine learning can help in predicting future emission trends for informed policy-making and sustainability efforts.

![image](https://github.com/user-attachments/assets/50235afc-9928-4f6c-92f3-c744f342fd67)

### Problem Statement:

Analysis of country-specific data and development of machine learning models in order to predict CO2 emissions from country parameters. The project uses the publicly available dataset Climate Change Data from the World Bank Group, which provides data on the vast majority of countries over a range of years for parameters such as:

- country: the vast majority of countries worldwide
- year: ranging from 1990 to 2011
- various emissions of greenhouse gases such as CO2, CH4, N2O, others
- population-specific parameters: population count, urban population, population growth, etc.
- country economic indicators: GDP, GNI, Foreign Direct Investment, etc.
- land-related parameters: cereal yield, agricultural land, Nationally terrestrial protected areas, etc.
- climate data: precipitations, national disasters, etc.
- energy use
- counts of certain types of medical personnel
- etc.

**The project is divided into two stages:**
- Data cleaning and preparation
- Data exploration and Predictive analysis


### Stage 1: Data cleaning and preparation

**Notebook Contents:**
1. Introduction - project and notebook summary, notes on the data source
2. Notebook setup - libraries and data import
3. Global data overview
4. Definition of the initial project goals
5. Data cleaning
    - dealing with missing values
    - transformation of the columns into a numerical data type
    - renaming of features
    - removing empty columns and rows
6. Data frame transformation
    - melting of the data for each variable
    - integration of the data into a suitable data frame format
7. Removal of missing values
    - detection of missing values
    - removal of missing values by filtering the columns and rows, so that minimal amount of features and rows are lost
8. Export the clean data frame to a file

### Data source
The used data comes from the Climate Change Data of the World Bank Group, which provides country-specific data on parameters such as CO2 emissions, energy use, population count, urban population, cereal yield, nationally terrestrial protected areas, GDP, GNI, etc.

The dataset is publicly available at https://datacatalog.worldbank.org/dataset/climate-change-data and licenced under the Creative Commons Attribution 4.0 International license.


## 📊 Key Learning Areas:
### ✅ 1. Problem Understanding
- Carbon emissions are a key driver of climate change

- Predicting them can help reduce environmental impact and plan better energy policies

- Use data science as a tool to contribute toward Sustainable Development Goals (SDG 13 – Climate Action)

### ✅ 2. Dataset Introduction
- Global CO₂ emissions data from various sources (e.g., World Bank, Our World in Data, Kaggle)

- Key columns likely included:

    - Year

    - CO2_Emissions_per_Capita

    - Population

    - Energy_Use

    - GDP

### ✅ 3. Tools & Libraries Introduced
- Python

- Pandas, NumPy for data handling

- Matplotlib, Seaborn for visualizations

- Scikit-learn for initial model setup

### ✅ 4. Tasks Performed in Week 1
- Imported and explored the dataset

- Checked for missing values, nulls, and data types

- Performed basic visualizations (e.g., line plots of CO₂ over time)

- Understood correlations between variables


## Links 
**github link for 1st week code : https://github.com/RGS-AI/AICTE_Internships/blob/main/2025/June_2025/Carbon_Emission_Prediction/1_data_preparation.ipynb**

**drive link for 1st week code : https://colab.research.google.com/drive/1uYvbmIZvQRD3vBZqrVfkegsjWYeWtliI?usp=drive_link**

.
-
.
# WEEK 2 : Model Building and Training
### 🎯 Goal for Week 2:
To build, train, and evaluate machine learning models (like Random Forest) that can accurately predict CO₂ emissions using real-world data.

### Prediction of CO2 emissions from country-specific data
![image](https://github.com/user-attachments/assets/28167d39-b30e-4307-92fa-1ad801f2555a)

### Stage 2: Data exploration and visualization
**Notebook Contents:**
0. Introduction
1. Notebook setup - libraries and data import, notes on the data source
2. Global data overview
3. Feature/column abbreviations and units
4. Definition of the hypothesis to be tested
5. Feature engineering
- features overview
- derivation of additional important features
- removal of unnecessary features
6. Prepare the visualization
7. Create plots
- a global look onto all relationships and detailed plots of chosen dependencies
- correlation matrix heatmaps
- scatterplots, histograms
- detection of outliers
- discussion of dependencies and trends
8. Conclusions

### 🔹 1. Model Selection
- Chose appropriate regression models:
        - Random Forest Regressor (main model)
        - Possibly tried Linear Regression or Decision Tree for comparison

### 🔹 2. Data Splitting
- Used train_test_split() to divide data:
        - 80% training, 20% testing
        - Example:

        from sklearn.model_selection import train_test_split
        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
  
### 🔹 3. Model Training
- Trained the model using:

        model = RandomForestRegressor()
        model.fit(X_train, y_train)
- Learned how the model "learns patterns" from features like:
        - Population
        - Energy consumption
        - GDP

### 🔹 4. Evaluation Metrics
- Evaluated model performance using:
        - R² Score (explains variance)
        - RMSE (root mean squared error)

        from sklearn.metrics import r2_score, mean_squared_error
        
        r2 = r2_score(y_test, y_pred)
        rmse = mean_squared_error(y_test, y_pred, squared=False)
### 🔹 5. Visualization
- Plotted Actual vs Predicted CO₂ Emission
- Created correlation plots to interpret performance
- Identified which features had the most influence on emissions

## Links 
**github link for 1st week code : https://github.com/RGS-AI/AICTE_Internships/blob/main/2025/June_2025/Carbon_Emission_Prediction/2_data_preparation.ipynb**

**drive link for 1st week code :[ https://colab.research.google.com/drive/1uYvbmIZvQRD3vBZqrVfkegsjWYeWtliI?usp=drive_link](https://colab.research.google.com/drive/12AOcLgfnui_5XKyVm6uq0hWZ3qI5psh0?usp=drive_link)**

.
-
.

# 📘 Week 3 : Model Optimization, Forecasting & Reporting

### 🎯 Goal for Week 3:
To improve model performance through tuning, forecast future CO₂ emissions, visualize results, and prepare final reports and presentations.

## Predictive data analysis with the Random Forest machine learning algorithm
![image](https://github.com/user-attachments/assets/92b32c3a-98d6-4f7f-aa55-b4592146bf9a)

### Stage 3 Notebook Contents:
0. Introduction - project and notebook summaries, notes on the data source
1. Notebook setup - libraries and data import, dealing with randomness in the algorithms
2. Data overview
3. Used feature/column abbreviations
4. Hypothesis to be tested
5. Selection of dependent and independent variables
6. Dataset splitting into training and testing subsets
7. Feature selection with recursive feature elimination and cross-validation
8. Hyperparameter tuning of a random forest model with cross-validation
9. Train and evaluate the model with the best hyperparameters on the training data with cross-validation
10. Validate the model on the test subset (previously unseen data)
11. Conclusions

## ✅ Key Learning Areas in Week 3:
###🔹 1. Hyperparameter Tuning
- Used GridSearchCV or RandomizedSearchCV to find the best parameters:
        
        from sklearn.model_selection import GridSearchCV
        
        param_grid = {
            'n_estimators': [100, 200, 300],
            'max_depth': [10, 20, None]
        }
        
        grid = GridSearchCV(RandomForestRegressor(), param_grid, cv=5)
        grid.fit(X_train, y_train)
        
        best_model = grid.best_estimator_
- Learned how tuning improves accuracy and prevents overfitting

### 🔹 2. Cross-Validation
- Applied k-fold cross-validation (usually 5 or 10 folds)

- Ensured stable performance across multiple data splits

### 🔹 3. Future Forecasting (2010–2030)
- Predicted CO₂ emissions for future years using trained model
- Input values were extrapolated (e.g., population, energy use trends)

- Forecast Example:
        - 2025: 34,500 metric tons
        - 2030: 36,000 metric tons

### 🔹 4. Final Visualization
- Created:
        - Line plot for actual vs predicted emissions
        - Feature importance graph
        - Forecast graph (2010–2030)

### 🔹 5. Final Documentation & Presentation
- Prepared:
        - PowerPoint presentation (slides: problem, tools, EDA, model, output)
        - Project report or PDF
        - Screenshots of:
                - Code
                - EDA
                - Model output
                - Evaluation metrics
                - Prediction charts

## Links 
**github link for 1st week code : https://github.com/RGS-AI/AICTE_Internships/blob/main/2025/June_2025/Carbon_Emission_Prediction/3_data_preparation.ipynb**

**drive link for 1st week code :[[ https://colab.research.google.com/drive/1uYvbmIZvQRD3vBZqrVfkegsjWYeWtliI?usp=drive_link](https://colab.research.google.com/drive/12AOcLgfnui_5XKyVm6uq0hWZ3qI5psh0?usp=drive_link)](https://colab.research.google.com/drive/1UKqUbTd-iF4AhdaNDB5Id8dL68DVxnFv?usp=drive_link)**
