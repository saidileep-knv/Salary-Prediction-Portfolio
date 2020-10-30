# Salary-Prediction-Portfolio
Salary Prediction Project (Python)

## Methods Used
* Data Analysis and Visualization
    * Model Building
        * Linear Regression
        * Polynomial Transformation
        * Ridge Regression
        * Random Forest
        * Gradient Boosting
## Technologies/Libraries Used
* Python 3
* pandas
* NumPy
* seaborn
* scikit-learn
* matplotlib
* SciPy
* Jupyter

# Description
The purpose of this project is to use data transformation and machine learning to create a model that will predict a salary when given years of experience, job type, college degree, college major, industry, and miles from a metropolis.

# Data
The data for this model is fairly simplified as it has very few missing pieces. The raw data consists of a training dataset with the features listed above and their corresponding salaries. Twenty percent of this training dataset was split into a test dataset with corresponding salaries.

There is also a testing dataset that does not have any salary information available and was used as a substitute for real-world data.

## Information Used To Predict Salaries
Variable            | Description
--------------------| ---------------------
jobId               | Given JobID for the role
companyId           | CompanyID for the respective jobId advertised
degree              | Applicant's qualification
major               | Degree specialization
industry            | JobId's categorized industry such as Oil, Auto, Health, Finance, etc., 
yearsExperience     | Required Experience for the role
milesFromMetropolis | Distance of the job location in miles from the nearest metropolitan city
salary              | In x1000 dollars of the respective jobId

# Summary
Applying second order polynomial transformation to the features used gave the most accurate predictions with the least error when using a linear regression model. The result was a mean squared error of 353 and r-squared of 0.764.

This model can provide the most accurate results when supplied with information on yearsExperience, milesFromMetropolis, jobType, degree and major.
