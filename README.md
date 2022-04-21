# Predictive-Maintenance
 M.Tech Final year project

Data Source Link: https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification

Webapp Link: https://share.streamlit.io/dkc-7000001/predictive-maintenance/main/predict_page.py

### Data Understanding:-

#### This dataset reflects real predictive maintenance encountered in the industry to the best of our knowledge. And i am going to use this to predict the failure and by getting that info we can predict the requirment of maintenance. and with that we can save money and effort.

## Steps

### <-- Step1 -->---------------->>>Data collection and preprocessing<<<

As the data has no null values, there is not much required in data preprocessing.

### <-- Step2 -->---------------->>>Model Building<<<

Here there are two target variables, one of it was of binary (Failure) class and one of it was of multi class (Type of failure) feature variable. I have tried different types of ML algorithm, and found that RandomForest Classifier was giving the best performance with almost 99.5% of accuracy. There is cache in this project, that as there are two target variables, so i have used two RandomForest Classifier to predict both the target variable, and i also taken care that none of the variable is used to predict the other target variable, which will leads to memory leak problem.

### <-- Step3 -->---------------->>>Dumping Model<<<

After building both the model , both has been dumped into a pickle file to use again into the webapp to predict the failure which will help us to schedule the maintenance.

### <-- Step4 -->---------------->>>Building Webapp<<<

With the help of Streamlit library, a basic Webapp has been build, Asking 5 questions from user to predict the failure.



