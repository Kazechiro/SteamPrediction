# SteamPrediction - Steam Store Games Dataset


## Overview
This document provides a detailed description of the "Steam Store Games" dataset, which contains information about games available on the Steam platform. The dataset will be used for predictions with KNN, logistic regression, decision tree, random forest, and support vector classifier (SVC) models.

## Note
This analysis is conducted by a student still in the learning process, so it may contain some errors, if you find any error feel free to make a a pull request.

### Dataset Link
[Steam Store Games Dataset on Kaggle](https://www.kaggle.com/datasets/nikdavis/steam-store-games)

## Dataset Structure
The dataset contains the following variables:

| **Column**           | **Description**                                                                                     | **Importance**                                                                                                                                                   |
|----------------------|----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `appid`              | Unique identifier for each game.                                                                   | Essential for specific references and data cross-checking.                                                                                                      |
| `name`               | Name of the game.                                                                                  | Fundamental for identification and search. Influences perception and game marketing.                                                                             |
| `release_date`       | Release date in the format YYYY-MM-DD.                                                             | Useful for analyzing trends over time.                                                                                                                          |
| `english`            | English language support (1 for yes, 0 for no).                                                   | Helps understand the target market and game accessibility.                                                                                                      |
| `developer`          | Name(s) of the developer(s).                                                                       | Can influence consumer trust and marketing.                                                                                                                     |
| `publisher`          | Name(s) of the publisher(s).                                                                       | Affects visibility and success of the game.                                                                                                                     |
| `platforms`          | List of supported platforms (Windows, Mac, Linux).                                                | Helps identify the game's accessibility.                                                                                                                        |
| `required_age`       | Minimum age requirement according to PEGI standards.                                              | Essential for understanding the target audience and meeting classification regulations.                                                                          |
| `categories`         | List of game categories (e.g., single-player, multiplayer).                                        | Facilitates categorization and game search.                                                                                                                     |
| `genres`             | List of game genres (e.g., action, adventure).                                                    | Crucial for market and trend analysis.                                                                                                                          |
| `steamspy_tags`      | List of community-voted tags.                                                                      | Provides insights into how the community perceives the game.                                                                                                    |
| `achievements`       | Number of in-game achievements.                                                                   | May impact player engagement and satisfaction.                                                                                                                  |
| `positive_ratings`   | Number of positive reviews.                                                                        | Indicator of the game's reception by the audience.                                                                                                              |
| `negative_ratings`   | Number of negative reviews.                                                                        | Helps understand criticism of the game.                                                                                                                         |
| `average_playtime`   | Users' average playtime.                                                                           | Engagement indicator.                                                                                                                                           |
| `median_playtime`    | Users' median playtime.                                                                            | Provides a more stable view of engagement.                                                                                                                      |
| `owners`             | Estimated number of owners, with lower and upper bounds.                                          | Indicates the game's popularity.                                                                                                                                |
| `price`              | Current price of the title in GBP.                                                                | Crucial factor in purchase decisions and revenue analysis.                                                                                                       |

## Analysis Applications
The variables in this dataset can be used for various analyses, such as:
- **Trend Analysis:** Examine the popularity of game genres or types over time.
- **Revenue Analysis:** Correlate price and number of owners to understand how price changes affect sales.
- **Quality Assessment:** Compare positive and negative reviews to identify which developers or genres are best received.
- **Market Segmentation:** Identify user segments based on categories and supported platforms.

## Analysis Objective
The primary goal of this project is to predict the **positive_ratings** variable to understand the factors influencing positive reviews for a game.

## Models to Be Used
The prediction will be carried out using the following models:
- **KNN (K-Nearest Neighbors):** A method that classifies a point based on the class of its closest neighbors.
- **Logistic Regression:** A statistical model that uses the logistic function to model the probability of a class or event.
- **Decision Tree:** A model that uses a tree-like graph to make decisions based on game features.
- **Random Forest:** An ensemble of decision trees that improves prediction accuracy by reducing overfitting.
- **Support Vector Classifier (SVC):** A model that classifies data by finding the hyperplane that best separates different classes.

## Data Preprocessing
The data preprocessing will include:
- Handling missing values.
- Encoding categorical variables.
- Normalizing or standardizing the data, if necessary.

## Exploratory Data Analysis
During the data exploration phase, the following will be performed:
- Visualizations to understand data distribution.
- Correlation analysis between variables.

## Conclusion
This dataset provides a comprehensive view of the Steam games ecosystem. This notebook aims to predict the **positive_ratings** variable to uncover what drives players to rate a game positively.
