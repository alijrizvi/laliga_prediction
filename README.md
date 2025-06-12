# La Liga Match Outcome Prediction

## Project Overview
This project aims to predict the outcomes of La Liga football (soccer) matches. By leveraging historical match data, various machine learning models are trained and evaluated to provide insights into potential match results. The goal is to build a robust prediction system that can assist in understanding game dynamics and potential future outcomes.

* Table of Contents
* Project Overview
* Table of Contents
* Motivation
* Data Sources
* Methodology
* Results and Discussion
* Credits
* License

## Motivation
The motivation behind this project stems from a keen interest in combining a passion for Data Science as a professional Data Analyst and aspiring Data Scientist with football - and sports overall - and the desire to apply machine learning techniques to real-world sporting events. Predicting match outcomes is a challenging task due to the numerous variables and inherent randomness in sports. This project serves as an exploration into building predictive models for La Liga, offering insights into factors that influence a team's long-term trajectory.

## Data Sources
The primary data source for this project consists of historical La Liga match data from *FBRef.com*. This data typically includes:

- Season of Team's Matches Played
- Team statistics (e.g., Wins, Draws, Losses, xG/90 since this statistic was recorded)

## Methodology
The project follows a typical machine learning pipeline:

- Data Collection and Preprocessing: Historical and this Season's up-until-now La Liga match data is collected and cleaned. This involves handling missing values, converting data types, and feature engineering to create relevant predictors.
Feature Engineering: New features are created from raw data, such as:
-- pts/mp (Points per Match)
- Exploratory Data Analysis (EDA) & Visualization: Initial analysis and visualization of the data is performed to understand distributions, relationships between variables, and identify potential trends.
- Model Selection: Various machine learning algorithms are explored for classification tasks (predicting Home Win, Draw, or Away Win). Common algorithms considered include:
-- Random Forests Classifier
-- Logistic Regression
-- Linear Regression and Regularized Linear Models (L1/Lasso and L2/Ridge)
- Model Training and Evaluation: Selected models are trained on historical data. Cross-validation techniques are employed to ensure model robustness. Performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.
- Prediction: The trained model is used to predict outcomes for future matches.

## Results and Discussion
- The Random Forests Classifier very neatly calculated each Team's chances of winning the League this season, out of a sum-total of 100% for the entire league.
- Logistic Regression proved very accurate in predicting whether a Team would end up Champion or not, based on its current performance metrics.
- Both, the L1 Regularized and L2 Regularized Linear Model, performed very well in terms of predictive accuracy after extracting out optimal features and tuning all features, respectively.
- Wins and Points per match proved to be the most important predictors of total points earned in the future.
- No biases were discovered in the Training and Testing of models.

## Credits
A significant portion of this project, specifically more than half of the conceptualization and implementation, was inspired by and directly adapted from the excellent tutorials and insights provided by Anas Riad on his YouTube channel. His work was instrumental in guiding the development of the data processing and model building aspects of this project.

### License
This project is licensed under the MIT License - see the LICENSE file for details.
