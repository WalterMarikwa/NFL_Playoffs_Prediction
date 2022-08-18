# NFL Playoffs Prediction

## Overview

Gathering data to analyze and calculate NFL passing and rushing team stats to come up with a fair assumption on which team is most likely going to make it into the playoffs for the 2022/23 season. 

Each team member has taken on a role as outlined in the module guidelines. A slack channel has been created for team members to collaborate and update each other on the status of their contribution and ask for team member input when needed.  

## Resources

Tools: Python 3, Jupyter Notebook, Pg Admin4, PostgreSQL.

Data source: [cleaned_offense](cleaned_offense.csv)
  - The origin of this dataset was pulled from [NFL Table](https://www.nfl.com/stats/team-stats/offense/passing/2021/reg/all) by web scraping. Afterwards the data was loaded into a database where we validated it and made sure it's ready for our machine learning model connection.


## Purpose

This analysis will entail the prediction of our machine learning and report a detailed outcome and the statistical findings. The teams in our data will be classified as being playoff contenders or not, so we have decided to go with a decision tree model.

Our mockup, as shown below, contains the steps for a decision tree model. We have preprocessed the data by dropping any null rows and any columns that do not contain data suitable for the model, including non-numeric data. The decision tree model will take our data (statistics) and run through each one until the team is classified as playoffs or not. We felt this was the most appropriate model because of the step by step approach that decision trees take. The training and testing data was split into the standard 75%/25% ratio. After training and testing our data, we will analyze the confusion matrix to ensure that the accuracy is sufficient for us to move forward with the model as is.

Our target accuracy is 70%. If the model does not meet our accuracy needs, then we can test on an updated model.

![](https://github.com/WalterMarikwa/UNCC_Final_Project_Capstone/blob/kf_branch/images/model_mockup.png)



