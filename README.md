# Predicting West Nile Virus

This was a team project with the goal of creating a cost benefit analysis of when and where the city of Chicago could spray pesticides in order to reduce the affect of West Nile virus on humans. We began by researching effective surveillance techniques and the best predictors of West Nile virus. While we conducted much of our EDA on a dataset given to us from Kaggle, we ultimately retrieved mosquito trap data for the last 12 years from the city of Chicago website along with weather data for those years from the NOAA. Using the data, we oversampled positive cases in order to create a model that was sensitive to its presence. To avoid overfitting on sparse data, we used a random forest with a small depth to predict the dates and locations of mosquitoes with the disease. Taking into account areas with dense susceptible populations, the predictions of our model, and the cost of spraying, we created our recommendations for the city of Chicago.

This repo only includes the files I created for this project. It has notebooks used to go from the new data sets through the creation of the final model. While it does not include much of the EDA on the original dataset, the decisions made were often based on that EDA.

How to explore this repo:
- The assets folder includes the data and predictions
  - The mosquito files include the trap data on mosquito and West Nile virus locations taken from the city of Chicago website
  - The weather files are from the NOAA for the same time period
  - The "real" files are the actual locations of West Nile virus for the test data
  - The "predictions" files are the predicted locations of West Nile virus for the test data
- The west nile (and input) folder has the data used for the project
- The data cleaning file is a basic preparation of the files to be ready for feature engineering
- The feature engineering file is used to create the features based on our research and EDA
- The model file includes the model and its results

