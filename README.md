# NBA Team Metrics Analysis Project
## Introduction
This project aims to analyze NBA team metrics from the regular seasons ending in 2021, 2022, and 2023 to identify the key performance indicators that correlate with regular season wins. By exploring this comprehensive dataset sourced from Basketball Reference, we hope to uncover insights that teams can use to enhance their chances of success.

## Group Members
Braulio Duran (bdura2)
Isabella Linarez (ilina2)
Basim Nabulsi (basimsn2)
Moe Abuseini (mabus3)
Sebastian Kowalczyk (skowa3)

## Data Source
The data used in this analysis was sourced from:

NBA 2021 Season
NBA 2022 Season
NBA 2023 Season
1st Half of NBA 2024 Season

## Data Cleaning
The dataset was relatively clean with no null values.
Manually added W/L% from other tables.
Removed "*" from team names.
Removed the last column containing league averages as they were insignificant to the analysis.

## Exploratory Data Analysis (EDA) and Visualizations
Correlation Analysis: We calculated the correlation of various team metrics with win/loss percentage (W/L%) and identified key performance metrics.
Hypothesis 1: There is a positive correlation between Field Goal Percentage (FG%) and Win Percentage (W/L%).
Hypothesis 2: There is a negative correlation between Turnovers (TOV) and Win Percentage (W/L%).
Machine Learning Analysis
A Logistic Regression model was used to predict win/loss percentages.
Feature selection identified the most relevant metrics, such as 3P%, PTS, FG%, DRB, and FT.
The model was trained on the first half of the 2023-24 season and achieved an accuracy of 90% when tested on the second half.

## Hypothesis Testing
Hypothesis 1: Higher FG% leads to higher W/L%.
Pearson correlation coefficient: 0.607
P-value: < 0.05 (significant)
Conclusion: We reject the null hypothesis, indicating a strong positive correlation.
Hypothesis 2: Higher 3PT% leads to higher W/L%.
Pearson correlation coefficient: 0.666
P-value: 7.604e-13 (significant)
Conclusion: We reject the null hypothesis, indicating a strong positive correlation.
Overall Results
Metrics such as 3P%, 3PA, and FG% strongly correlate with team success in the NBA.
Teams focusing on improving shooting efficiency and reducing turnovers are more likely to achieve higher win percentages.

# How to Run the Code
## Install Dependencies:
pip install pandas seaborn matplotlib scipy scikit-learn

## Run the Analysis:
Load and clean the data using the provided CSV files.
Perform EDA and visualizations using the code in the EDA section.
Execute the machine learning analysis for predictive modeling.
Conduct hypothesis testing to validate the findings.

## Functions:
myFunctions.clean_data: Cleans the data from CSV files.
myFunctions.find_most_important_metric: Calculates correlation between metrics and W/L%.
myFunctions.bar_plot_correlation: Generates a bar plot of correlations.
myFunctions.clean_season_halfs: Splits the season data into halves.
myFunctions.train_and_predict: Trains the Logistic Regression model and predicts outcomes.
