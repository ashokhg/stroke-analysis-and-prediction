# Stroke_Analysis_and_Prediction
Use of Machine Learning and Tableau Dashboards to Help Predict Strokes and Understand Contributing Factors

## Objective
To develop a model which can reliably predict the likelihood of a stroke using patient input information.

## Programs Used
<p>•  Python </p>
<p>•  Pandas <p/>
<p>•  Jupyter Notebook </p>
<p>•  JavaScript </p>
<p>•  scikit-learn </p>
<p>•  imbalanced-learn </p>


## Hypothesis
Hypothesis: A reliable predictive model can be developed if the data and stroke key attributes are correctly identified and prepared for the machine learning process.

## Data
Data is from Kaggle [6]


## Data Exploring
Most of the data was biased in the histograms, except for age and Residence_type. For the Yes/No questions, the data was left biased correlating to 0 which presents No as the answer to the respective question.   The attributes bmi and average_glucose_level were left biased representing the lower end of their broad spectrum of data points. 
<br>
<br>

## Machine Model Evaluation
The primary objectives of the model evaluation process were to identify a model that did not overfit the data, generated the highest f1-score for 1 (“Yes” for stroke) and generated the highest recall for “Yes”.  The large number of 0 values (“No” for stroke), ensured a good f1-score for 0, but our objective was to identify a model that will give the best “Yes” result.  That presented a challenge for the models.  As noted above, SMOTE was used to help with this issue.

### Linear Models

Models evaluated were LogisticRegression, KNeighborsClassifier and Support Vector Machines (svm).  

The best results for the linear model was LogisticRegression with an Out Sample f1-score of 0.23.  KNeighborsClassifier and svm gave 0.16 and 0.19, respectively.


## Feature Importance
Feature importance is presented below.  The chart presents the assigned value of the relationship between stroke and identified attribute.  Like the correlation heat map, the values closer to zero indicate minimal to no linear relationship.  

## Conclusion
Objective: To determine if a reliable model was developed, the risk factors identified by the American Stroke Association will be compared against the Features Importance table and live data will be tested.

Revisiting the Hypothesis criteria

Basis Risk Factors from American Stroke Association common to the dataset.
<p>•  High Blood Pressure</p>
<p>•  Smoking</p>
<p>•  Diabetes</p>
<p>•  Obesity</p>
<p>•  Heart Disease</p> 
<p>•  Age (cannot be controlled)</p>
<p>•  Gender (cannot be controlled)</p>


## References
[1] Ahmad FB, Cisewski JA, Miniño A, Anderson RN. Provisional Mortality Data — United States, 2020. MMWR Morb Mortal Wkly Rep 2021;70:519–522. DOI https://www.cdc.gov/mmwr/volumes/70/wr/mm7014e1.htm?s_cid=mm7014e1_w#F1_down

[2] American Stroke Association, https://www.stroke.org/en/about-stroke/types-of-stroke/ischemic-stroke-clots

[3] American Stroke Association, https://www.stroke.org/en/about-stroke/types-of-stroke/hemorrhagic-strokes-bleeds

[4] American Stroke Association, Explaining Stroke, pages 1-20, https://www.stroke.org/-/media/stroke-files/stroke-resource-center/brochures/explaining_stroke_brochure_6_25_19.pdf?la=en

[5] American Stroke Association, https://www.stroke.org/en/about-stroke

[6] Stroke Prediction Dataset, 11 clinical features por predicting stroke events, https://www.kaggle.com/fedesoriano/stroke-prediction-dataset

[7] Stroke Mortality Data Among US Adults (35+) by State…2016, Dataset in U.S. Department of Health & Human Services, https://data.world/us-hhs-gov/12ea7a13-b229-43b4-b19b-1459e9a64d3f

[8] USDA Economic Research Service, U.S. Department of Agriculture, https://www.ers.usda.gov/data-products/county-level-data-sets/download-data/

[9] Centers for Disease Control and Prevention, National Center for Health Statistics, https://www.cdc.gov/nchs/nhis/tobacco/tobacco_glossary.htm

