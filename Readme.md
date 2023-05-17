# Sanity-Test
A dataset containing various attributes that impact the result of the sanity test was given and when a particular file in the given directory changes and is committed to GitHub. A classification model was built to predict if a sanity test case will fail on the platform for a given combination of attributes when a particular file is changed. The model is enhanced to identify the scenarios which have a very low probability of failure for the change in a
particular set of files.

FLOWCHART
![image](https://user-images.githubusercontent.com/99869699/232679766-9716717d-c1f9-46b6-aff5-7908e83ba6a8.png)

PROPOSED MODEL
![image](https://user-images.githubusercontent.com/99869699/232679877-c938edca-207c-4852-b36c-20f17eff7e96.png)

ANALYSIS

This was a multiclass classification problem. 

We founded the correlation matrix in this problem statement and concluded that output was dependent on all the attributes.

Some attributes in the dataset were given as english texts so, in order to train our machine learning model we vectorized all of the attributes. Here we used NLP for the process of vectorization.

![image](https://user-images.githubusercontent.com/99869699/232680145-55cdb0ad-25fe-4a1b-b91f-0b2aa28a673b.png)

After researching deeply we choose to apply “Bag Of Words” on the attributes whose count of unique value (categories) > 20.

We applies “Bag of words” on three attributes which were: 

File changed

Component

Sanity name

For attributes whose count of unique value (categories) < 20, we applies “One Hot Encoding”.

![image](https://user-images.githubusercontent.com/99869699/232680232-b5160296-19c7-4cef-9eb8-4cedf6352ddc.png)

After preprocessing the data, finally the dataset looked like this
<img width="644" alt="image" src="https://user-images.githubusercontent.com/99869699/232680375-e1a77fbc-07fc-4065-b84e-a1ce6402763e.png">

After applying different classification models like XGBoost, Naive Bayes, Decision Tree, Multinomial logistic regression, the accuracy of the proposed model is listed below. 

<img width="574" alt="image" src="https://user-images.githubusercontent.com/99869699/232680904-bec523e7-79e9-4b92-9b70-893e14f61e62.png">

OUTPUT
![image](https://user-images.githubusercontent.com/99869699/232681022-2431fba1-434f-45e1-9021-ff088463f0cf.png)


