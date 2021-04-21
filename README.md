# Predicting User Churn for  a Music Streaming App

### Table of Contents

1. [Project Motivation](#motivation)
2. [File Descriptions](#files)
3. [Installation](#installation)
4. [Results](#results)
5. [Acknowledgements](#licensing)


## Project Motivation<a name="motivation"></a>

This project analysis a music streaming service's user data, looks at a random subset of the user data to predict which users will cancel the service (defined here as 'churn').  The subset contains 286,500 individual records and includes both categorical and numeric features.  

In pursuing this analysis, several key questions were asked:

1. What factors about individual usage contribute indicate churn?
2. How does gender play a role in churn rate i.e due males cancel at higher rates than females?
3. Are there features that may indicate the 'value proposition' of the streaming service to churn versus no churn users?


## File Descriptions <a name="files"></a>

There is one (1) notebook  and two text files available here to showcase work related to the above questions.
1. Sparkify.ipynb -  This jupyter notebook contains both exploratory analysis and modeling information
2. requirements.txt - A listing of all libraries and dependencies required to run the notebook analysis
3. README.md - An explanation of the repository contents and an overview of the analysis


## Installation <a name="installation"></a>

All required installations and dependencies are indicated in the requirements.txt file. More generally the jupyter notebook uses python, pyspark, pandas and classification models. The code should run with using Python versions 3.*.

## Results<a name="results"></a>

While the dataset contained only 61 days worth of data for 362 unique users, based on the exploratory analysis it was clear that most churn activity occurred within the first 40 days. In addition, churn users tended to be more erratic in the number of songs player per time period and most churn events (cancellations) tend to peak in the first 3 days of a month.  A more detailed analysis is provided at the following link [- click here](tbd).

Given that determining churn vs no_churn of the individual user is a binary classification problem, we chose to look at our data in aggregate based on individual users (compared to aggregate of single session data) and we used both a logistic regression model and a decision tree classifier.
## Acknowledgements<a name="licensing"></a>

The data used was taken from Udacity's Data Science Capstone project.  Further detailed information was used from the pyspark and python documentation sites.
