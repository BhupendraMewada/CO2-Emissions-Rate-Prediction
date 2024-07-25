# CO2 Emissions Prediction Using Machine Learning

## Project Overview
This LHL capstone project aims to predict CO2 emissions for any location based on geographical coordinates (latitude and longitude) and population data. The increasing global CO2 emissions due to human activities such as deforestation and fossil fuel consumption have motivated the hypothesis that a relationship exists between population metrics and CO2 emissions.

## Goal
The primary objective is to develop a predictive ML model to estimate the CO2 emissions rate for any location of interest, given its geographical coordinates and population data. The project also includes generating insights from the data and visualizing the results.

## Data
Data for this project was obtained from Kaggle under a free public license. The CO2 emissions dataset was integrated with geographical coordinates and population data from separate datasets:
- CO2 emissions dataset (no geographical coordinates)
- Latitude and longitude values dataset
- Population dataset

## Methods
1. **Data Integration & Cleaning:**
   - Mapped geographical coordinates to CO2 emissions data.
   - Merged population data with the integrated dataset.
   
2. **Exploratory Data Analysis (EDA):**
   - Visualizations in Tableau to explore data features and insights.
   - Correlation heatmap to identify key features (latitude showed highest correlation with CO2 emissions).
   
3. **Modeling:**
   - Built a baseline Linear Regression model (R-squared: 20%).
   - Trained and compared multiple models: Decision Tree, Random Forest, and XGBoost.
   - XGBoost model achieved the best performance (R-squared: 98%).

4. **Deployment:**
   - Deployed the model using Flask for local machine use.
   
## Results
- **Insights:** Latitude has a higher correlation with CO2 emissions than population density, possibly due to climatic preferences near the equator.
- **Model Performance:** XGBoost outperformed other models with an R-squared score of 98%, demonstrating the ability to predict CO2 emissions effectively.

## Challenges
The main challenge was data gathering, as CO2 emissions data is not readily available with population data.

## Future Goals
- Periodically update the dataset and experiment with additional models.
- Convert cleaning and preprocessing steps into a Python script to create a data pipeline.
- Deploy the model on a cloud platform such as AWS EC2.

## Tools & Technologies
- **Programming Languages:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost)
- **Visualization:** Tableau
- **Deployment:** Flask
