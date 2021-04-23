# Predicting User Churn for  a Music Streaming App

### Table of Contents

1. [Project Motivation](#motivation)
2. [Files In Repository and File Descriptions](#files)
3. [Libraries Used](#libraries)
4. [Results Summary](#results)
5. [Acknowledgements](#acknowledgements)


## Project Motivation<a name="motivation"></a>
A detailed discussion of this project may be found at https://khebel.medium.com/predicting-when-users-stop-listening-to-the-music-a506216a73e4.

2020 saw the acceleration of increased digital marketing and online spending. Given the drive toward increased profitability and improved customer retention, identifying those users that are most likely to cancel or not to return is a high priority. Creating programming, marketing or features to capture these users, can have substantial positive effects on overall profitability.

The following analysis addresses the issue of customer retention by predicting the likelihood of a user cancelling their subscription to a music streaming service. This analysis of users is based on a subset and includes 286,500 rows and 225 unique users using both paid and free levels of a music streaming service. The primary task is to identify users who will cancel the service. ‘Churn’ was defined as this cancellation action. With 62 days worth of information, the data was analyzed to determine features distinguishing the ‘churn’ user group from the ‘no-churn’ user group. This information was then used to create a machine learning model to make predictions on the likelihood any individual user will cancel their music subscription service.

In pursuing this analysis, several key questions were asked:

1. What factors about individual usage contribute indicate churn?
2. What machine learning predictive model works best for predicting churn?


## Files in Repository and File Descriptions <a name="files"></a>

There is one (1) notebook  and two text files available here to showcase work related to the above questions.
1. Sparkify.ipynb -  This jupyter notebook contains both exploratory analysis and modeling information
2. requirements.txt - A listing of all libraries and dependencies required to run the notebook analysis
3. README.md - An explanation of the repository contents and an overview of the analysis


## Libraries Used <a name="libraries"></a>

Libraries used for this project were: pyspark.sql (functions, types), numpy, pandas, datetime, matplotlib.pyplot,  pyspark.ml (classification, evaluation) and pyspark.mllib (evaluation).
All required installations and dependencies are indicated in the requirements.txt file.

## Results Summary <a name="results"></a>
Factors contributing to user churn include lower user engagement measured by the number of songs played over specific time periods and a prior upgrade or downgrade.  The random forest model was the best predictive model.

Random forest classifier results based on a normalized dataset were deemed successful both for the test and validation set with scores over 81%. This success can be attributed to the fact that with limited numerical features within the dataset, the model was able to optimize these features to find patterns of user behavior related to churn. Improvements to the model were made specifically my changing params, numTrees and maxDepth. It is worth noting that the standard scaled datasets performed much poor with the random forest classifier. It is assumed that this because the model needs greater variability in variables for variable weight importance. The standard scaled vectors strip this variability away making patterns harder to discern.

## Acknowledgements<a name="acknowledgements"></a>

The data used was taken from Udacity's Data Science Capstone project.  Further detailed information was used from the pyspark and python documentation sites.
