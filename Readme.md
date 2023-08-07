# Stroke_Analysis_and_Prediction
Use of Machine Learning to Help Predict Strokes and Understand Contributing Factors.

## Objective
To develop a model to predict the likelihood of a stroke using patient's health data as input.

## Libraries used
<p>•  Pandas <p>
<p>•  Jupyter Notebook </p>
<p>•  JavaScript </p>
<p>•  scikit-learn </p>
<p>•  imbalanced-learn </p>


## Hypothesis
Hypothesis: A reliable predictive model can be developed if the data and stroke key attributes are correctly identified and prepared for the machine learning process.

## Data
Dataset has taken from Kaggle

## Data Exploring
Most of the data was biased in the histograms, except for age and Residence_type. For the Yes/No questions, the data was left biased correlating to 0 which presents No as the answer to the respective question.   The attributes bmi and average_glucose_level were left biased representing the lower end of their broad spectrum of data points. 
<br>

## Machine Model Evaluation
The primary objectives of the model evaluation process were to identify a model that did not overfit the data, generated the highest f1-score for 1 (“Yes” for stroke) and generated the highest recall for “Yes”.  The large number of 0 values (“No” for stroke), ensured a good f1-score for 0, but our objective was to identify a model that will give the best “Yes” result.  That presented a challenge for the models.

### Linear Models

Models evaluated were LogisticRegression, KNeighborsClassifier and Support Vector Machines (svm).  

The best results for the linear model was LogisticRegression with an Out Sample f1-score of 0.23.  KNeighborsClassifier and svm gave 0.16 and 0.19, respectively.
 

### Conclusion
Objective: To determine if a reliable model was developed, the risk factors identified by the American Stroke Association will be compared against the Features Importance table and live data will be tested.
