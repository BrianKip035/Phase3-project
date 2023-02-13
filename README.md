
# Flu Shot Learning: Predicting Whether Individuals got their H1N1 Vaccines


This project aims to predict the likelihood of individuals receiving the H1N1 and seasonal flu vaccines by building a classification model using demographic, social, economic, and health-related data. The data used for this project is from the National 2009 H1N1 Flu Survey conducted in the United States.



# Business Understanding

The goal of this project is to understand the public's behavior towards receiving the flu vaccines and use that understanding to predict the likelihood of individuals receiving the H1N1 and seasonal flu vaccines. The success of the project will be measured by the accuracy, recall, and precision scores of the model.
## Main Objective

The main objective of this project is to develop a classification model to predict the response of individuals to H1N1 and seasonal flu vaccines.


Other Objectives

    1 Explore and visualize the data to gain a better understanding of the relationship between the variables and the target variable.
    2. Select and train different classification models, including logistic regression, decision trees, and random forest and evaluate their performance.
    3. To provide actionable insights for public health officials and policymakers to reduce the spread of contagious infections and promote herd immunity.





## Data Understanding

The provided dataset consists of 36 columns, with the first column being the respondent_id, which serves as a unique identifier. The remaining 35 features provide information about various aspects of the respondents, such as their:

    Level of concern and knowledge about the H1N1 flu
    Behavior towards the flu
    Recommendation of the H1N1 and seasonal flu vaccines by doctors
    Chronic medical conditions
    Contact with a child under six months

and many more.Most of the features are binary variables indicating yes or no, while some are multi-level variables representing different opinions, levels of concern, or knowledge.
## Data Preparation

Loading the Data
The necessary libraries were imported and the datasets were loaded into a Jupyter Notebook.
The data was examined for anomalies, outliers, missing values, and duplicates to determine the necessary steps to ensure the data was in a usable form. The training_set_features had a significant number of missing values, while the training_set_labels had no missing values and the test_set_features also had missing values. The data was then cleaned and pre-processed by filling in missing values, such as replacing missing values in the training_set_features with "Not Available".
##  Exploratory Data Analysis

Utilizing statistics and visualizations, the data sets were examined to identify trends that would make the data easier to understand. There were several questions that were answered in this step by comparing the predictor variables with the target variable which was expense (premium) using data visualization tools. The questions answered and variable relationships established include the following: 

    1. Does age_group affect the intake of H1N1 vaccine and seasonal_vaccine? 
    2. Does education affect the in_take of H1N1 vaccine and seasonal_vaccine? 
    3. Does Insurance affect the intake of H1N1 vaccine  and seasonal_vaccine?
    4. Does a region affect the intake of H1N1 vaccine and seasonal_vaccine ?
    5. Does employment_status affect the intake of H1N1 vaccine   and seasonal_vaccine?
    6. Does Race affect the intake of H1N1 vaccine and seasonal_vaccine ?

## Modeling



In this project, three machine learning algorithms were tested for their performance in predicting the likelihood of individuals getting the H1N1 and seasonal flu vaccines. The algorithms tested were logistic regression, decision trees, and random forest.

Data Preparation for Modeling 

Before testing the models, the data was split into training and testing sets, and the numerical features were scaled using the StandardScaler method, while the categorical features were encoded using the OrdinalEncoder method. This resulted in variables X_train, X_test, y_train, and y_test.

Model Evaluation

The accuracy, precision, recall, and overall entropy accuracy of each model were evaluated. The Random Forest model was found to be the best performer, with an accuracy of 84.9% for H1N1 and 78.5% for the seasonal flu vaccine. Logistic Regression had an accuracy of 81.3%, and Decision Trees had an accuracy of 77.9%. The overall entropy accuracy for both datasets combined was 0.78.

Final Model Selection
Based on the evaluation, the Random Forest model was selected for final evaluation on the test dataset due to its highest accuracy of 84.9% for H1N1 and 78.5% for the seasonal flu vaccine.
## Conclusion

Modeling

To predict H1N1 and seasonal flu vaccine behavior, three machine learning models were used: Decision Tree, Random Forest, and Logistic Regression. The models were developed using a pre-processed dataset that was split into training and testing sets, and the numerical features were scaled using StandardScaler while the categorical features were encoded using OrdinalEncoder.

Evaluation

The models were evaluated based on their accuracy, precision, and recall scores. The Random Forest model achieved the highest accuracy with 84.9% for H1N1 and 78.5% for the seasonal flu vaccine, while Logistic Regression had an accuracy of 81.3% and Decision Tree had an accuracy of 77.9%. The overall entropy accuracy for both datasets combined was 0.78. As a result, the Random Forest model was selected for final evaluation on the test dataset.
## Recommendations

ased on the project findings, here are some recommendations the public health sector could consider to improve vaccination rates:

Target vaccine education and communication efforts towards specific groups identified by the models as being hesitant or reluctant to vaccinate.
Develop tailored messaging and strategies that address concerns and barriers identified by the models.
Implement interventions that have been shown to be effective in improving vaccination rates, such as reminder systems, incentives, and reducing access barriers.
Conduct further research to identify and address factors that may not have been captured by the current models.
Use the models to forecast vaccine demand and allocate resources effectively to ensure that vaccines are available to those who need them.
Continuously monitor vaccination rates and adjust interventions as needed to ensure that vaccination goals are being met.  
curate it for a readme file
Recommendations for Improving Vaccination Rates
Based on the project's findings, the public health sector could consider the following recommendations to improve vaccination rates:

    1. Targeted Education and Communication: Focus vaccine education and communication efforts towards groups identified by the models as being hesitant or reluctant to vaccinate.

    2. Tailored Messaging and Strategies: Develop tailored messaging and strategies that address specific concerns and barriers identified by the models.
    3. Effective Interventions: Implement interventions such as reminder systems, incentives, and reducing access barriers, that have been shown to be effective in improving vaccination rates.

    4. Conduct further research to identify and address factors that may not have been captured by the current models.

    5. Use the models to forecast vaccine demand and allocate resources effectively to ensure that vaccines are available to those who need them.
    
    6. Continuously monitor vaccination rates and adjust interventions as needed to ensure that vaccination goals are being met.