# Terry Stop Arrest Predictor
![](https://images.unsplash.com/photo-1453873531674-2151bcd01707?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1973&q=80)



# Project Overview

## Key Business Problem

Build a classifier to predict whether an arrest was made after a Terry Stop, given information about the presence of weapons, the time of day of the call, etc. This is a binary classification problem.

## Stakeholders

Civil rights organizations: people who work to protect civil liberties and ensure fair treatment of individuals by law enforcement. They can use this classifier’s predictions to highlight potential biases or disproportionate targeting during the Terry Stops.

Law enforcement agencies: police departments, law enforcement agencies, particularly street crime units, and the narcotics units that are responsible for conducting Terry Stops. They could use the predictions to evaluate the effectiveness of their practices and identify areas for improvement in terms of increasing successful arrests or reducing false positives.

The general public: Anyone who is interested in civil rights and law enforcement practices. It could contribute to public discourse on policing methods and their impact on communities.

Data Scientists who are interested in working in law enforcement agencies.



## Data Understanding and Analysis
The overall goal is to come up with a binary classification model solution and to provide the top 2 features in this model.


## Source of data

[Terry Stops City of Seattle Open Data Portal](https://data.seattle.gov/Public-Safety/Terry-Stops/28ny-9ts8)

Description of Data:
This data represents records of police-reported stops under Terry v. Ohio, 392 U.S. 1 (1968). Each row represents a unique stop.
Each record contains the perceived demographics of the subject, as reported by the officer making the stop, and officer demographics as reported to the Seattle Police Department, for employment purposes.


## Visualizations (the same visualizations presented in the slides and notebook)
### Stops Arrest Background
![Stop Resolution](https://i.imgur.com/QIHetka.png)

![On-Site Physical Arrest Rate](https://i.imgur.com/Tu4UAPa.png)


#### Dummy Model Confusion Matrix
<img src="https://i.imgur.com/U0iMcKm.png" width=50% height=50%>

#### Dummy Model ROC Graph
<img src="https://i.imgur.com/SuhPw3o.png" width=50% height=50%>

#### Logistic Regression Model Confusion Matrix
![Logistic Regression Confusion Matrix](https://i.imgur.com/1rhuJUi.png)

#### Logistic Regression ROC Graph
![Logistic Regression ROC Graph](https://i.imgur.com/90tgyrj.png)

#### Logistic Regression Model Classification Report
<img src="https://i.imgur.com/CCbBb08.png" width=50% height=50%>

#### Decision Tree Model Confusion Matrix
![Decision Tree Confusion Matrix](https://i.imgur.com/666nZyR.png)

#### Decision Tree ROC Graph
![Decision Tree ROC Graph](https://i.imgur.com/uADJwfg.png)

#### Decision Tree Model Classification Report
<img src="https://i.imgur.com/0YO5YQw.png" width=50% height=50%>


## Conclusion
The decision Tree Classifier Model has the best performance to predict the arrest rate after a Terry stop. It yields an F1 score of 0.89.

The top features in this model are the arrest flag and frisk flag.

## Further Improvement
To further improve my model, I will use gridsearchCV for hyperparameter tuning to run my models in order to get a better F1 score.
I will also be looking into feature importance to see what are the important features of my model.
Also, applying other models, such as random forest, K-nearest neighbor.
