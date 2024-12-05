# Insurance Data Analysis

## Description

This project involves analyzing an insurance dataset to gain insights into factors influencing healthcare premium costs. The dataset contains information about policyholders and their claims, including their personal details, lifestyle choices, and medical conditions. The goal is to perform exploratory data analysis (EDA) to uncover patterns and correlations that will help create a predictive model for estimating medical insurance premiums.

ABC Insurance, the insurance agency, aims to analyze how different factors—such as body type, smoking status, age, and BMI—affect the premium costs. For example, smokers typically face higher premiums due to their increased likelihood of developing chronic diseases. This analysis will help the agency make informed decisions and improve their operations.

## Objective

To analyze the dataset and create a model that will predict medical insurance costs based on various input features.

## Dataset

The dataset used for this project is the `insurance.csv`, which contains the following features:

- **age**: Age of the person
- **sex**: Gender (Female or Male)
- **BMI**: BMI value to estimate an individual's health and fitness condition
- **children**: Number of children (1, 2, 3, 4, or 5)
- **smoker**: Whether the person is a smoker or not
- **region**: The region where the person resides (northeast, northwest, southeast, southwest)
- **charges**: The medical insurance charges (target variable)

## Project Steps

### 1. Import Libraries and Load Dataset

- Pandas, NumPy, Matplotlib, and Seaborn are used for data analysis and visualization.
- The `insurance.csv` file is loaded into a Pandas DataFrame for exploration.

### 2. Data Exploration

- **Data Shape and Types**: The initial step includes checking the shape of the dataset and the data types of each column to understand its structure.
- **Missing Values**: We examine if any columns have missing values and handle them accordingly.

### 3. Visualizing Relationships

- **Categorical vs Target Variable**: Count plots of categorical features such as `sex`, `smoker`, and `region` are analyzed in relation to the target variable `charges`.
- **Numerical vs Target Variable**: Scatter plots of numerical features like `age`, `BMI`, and `children` are explored to observe patterns in premium charges.
  
### 4. Observations from EDA

- **Gender Distribution**: The dataset is almost evenly distributed between genders, with 676 males (50.5%) and 662 females (49.5%).
- **Regional Distribution**: All four regions are represented approximately evenly in the dataset.
- **Children Distribution**: About 85% of the insured have fewer than 3 children.

### 5. Data Visualization

- **Feature vs Feature**: Various plots are used to explore relationships between different features, such as BMI vs charges, smoking status vs charges, and age vs charges.
- **Correlation Analysis**: A heatmap is created to understand the correlations between the features and the target variable (`charges`). The premium charges show a weak positive correlation with age and BMI, but a strong positive correlation with smoking status.

### 6. Advanced Analysis

- **Age vs Charges for Smokers and Non-Smokers**: We investigate whether the number of premium charges increases with age for smokers compared to non-smokers.

## Libraries Used

- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical computing.
- **Matplotlib**: Data visualization.
- **Seaborn**: Statistical data visualization.

## Future Work

- **Model Creation**: After performing thorough data exploration, we can proceed with creating machine learning models, such as Linear Regression, Decision Trees, or Random Forests, to predict medical insurance charges based on input features.
- **Model Evaluation**: Evaluate model performance using metrics like Mean Squared Error (MSE) and R-squared to assess how well the model predicts insurance premiums.

## Conclusion

This project provides valuable insights into how personal factors like age, BMI, and smoking status influence healthcare premiums. The findings can help ABC Insurance refine their pricing strategies, making them more data-driven and efficient.
