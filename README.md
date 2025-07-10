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
