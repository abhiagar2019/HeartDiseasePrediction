# HeartDiseasePrediction

Predicting Heart Disease from the set of three types of information, making a total of 13 features (orginal feature set was 74, but other features were deemed not important in several research studies). These 13 feautures could help explain the onset of a heart disease.
1) Demographics (such as age, sex)
2) Clinical information (such as cholesterol, blood sugar, thalassemia blood disorder) 
3) Test results (such as ECG, oldpeak etc)

13 Features are:

1. age: The person's age in years
2. sex: The person's sex (1 = male, 0 = female)
3. cp: The chest pain experienced (Value 1: typical angina, Value 2: atypical angina, Value 3: non-anginal pain, Value 4: asymptomatic)
4. trestbps: The person's resting blood pressure (mm Hg on admission to the hospital)
5. chol: The person's cholesterol measurement in mg/dl
6. fbs: The person's fasting blood sugar (> 120 mg/dl, 1 = true; 0 = false)
7. restecg: Resting electrocardiographic measurement (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy by Estes' criteria)
8. thalach: The person's maximum heart rate achieved
9. exang: Exercise induced angina (1 = yes; 0 = no)
10. oldpeak: ST depression induced by exercise relative to rest ('ST' relates to positions on the ECG plot. See more here)
11. slope: the slope of the peak exercise ST segment (Value 1: upsloping, Value 2: flat, Value 3: downsloping)
12. ca: The number of major vessels (0-3)
13. thal: A blood disorder called thalassemia (3 = normal; 6 = fixed defect; 7 = reversable defect)

target: Heart disease (0 = no, 1 = yes)


I am running multiple (8) base and grid searched classification models on
1.	All the 13 features provided
2.	Top 10 selected features (removing co-linear and features that were not highly correlated with the target variable)
3.	PCA with 8 components having 80% cumulative variance

So, in total 24 models were run to understand which model would provide the best results.

Girdsearched SVM comes out as the best model with cross validation score of 84% (FYI, base accuracy was 54%).

More detailed analysis coming soon. 
