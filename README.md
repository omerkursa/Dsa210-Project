# omerkursad DSA 210 Project

## Overview
This project aims to analyze my own spendings and see if the weather conditions or the temperature has any significant effects on my spendings.

## Proje Hedefleri
- Gain information about the data analysis techniques.
- Retrieve experience on data analysis

## Data Sources
- Visual Crossing Weather.
  Downloaded the weather data for Istanbul for the past 6 months.
- My own Akbank transaction data

## Step By Step
- In the first part of the project, finding the datasets were relatively easy. I extracted my own data from akbank mobile app and used it as my primary dataset.
- My second dataset came from a weather tracking NPO website. I downloaded the dataset including past 6 months. Please regard that 6 months was the maximum amount of data Akbank let me download.
- I used Google Colab for the whole project.
- Once I uploaded the datasets, I immedeately started cleaning my data. Removed unnecesary columns from the weather data and deleting no expense days from akbank data.
- Cleaning was not smooth as I thought since two datasets used a different date format which made me struggle among the whole project
- Than, I started Explanatory Data Analysis part.
- Displayed descriptive statistics, tried to find a correlation between datasets did normality tests, some other hypotesis testing and many many graphs.
- After all these, I started the machine learning part.
- Re-cleaned the data to avoid all possible biases
- Merged two datasets to work easier using the "date" parameter as a reference.
- Tried to do some feature engineering with minimum maximum expenses. I would like to categorize the expenses into more accuratte categories. However it was impossible to do the categorization because akbank didn't keep the categories. For example, for If I would like to create a category as coffee, many coffy shops was in the transactions and it was impossible to find each category and each shop for each category for me.
- Than, I started witha random forest algorithm to predict the weather condition wheras the input was the volume of transaction.
- As we all know, starting from april, past 6 months was mostly rainy, so my model had a 0.92 score predicting the rain. However due to lack of larger data, other predictions was not strong enough.
- Than I tried a random forest regressor and failed again. R^2 value was extremely low.
- I swithced my target and tried to predict the temperature with another regression model.
- However, either because lack of data or the lack of correlation, my model gave terrible results one again so I tried adding some min max features.
- Finally, I tried a kNN model. Found the optimal k value and retried.
- However, that model also failed to score.
- None of my models were able to explain the majority of the variance.

## Conclusion
- I learned a lot about datascience.
- Succesfully conducted data principles and applications.
- Somewhat have an idea about my spending habits.
- Learned Tried to apply ML algorithms.
- Learned that dataset construction was extraordinarily important in order to train and test a model.
- My dataset formats were not ideal to do the ML part, However, I tried my best.
- This experience tought me a lot.
