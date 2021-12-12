# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to figure out which modeling algorithm produces the most accurate results for credit card risk for the sample data set from Lending Club. This exercise is useful in finding out how credit card risk can be evaluated and therefore allowing lenders to make better decisions on whether or not to extend credit to applicants.

## Results
Naive Random Oversampling
Accuracy Score: 0.65
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145716686-6ff25f26-c4e6-4aac-8499-ac1e395dc8a7.png"> </p>

SMOTE Oversampling 
Accuracy Score: 0.64
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145717377-89da4904-6499-487e-940f-56f0ed49bfb7.png"> </p>

Undersampling with ClusterCentroids
Accuracy Score: 0.52
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145717515-ad1fa832-c292-4807-812f-13cb31a1e0a4.png"> </p>

Combination Sampling with SMOTEENN
Accuracy Score: 0.62
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145717765-e07c4003-a742-4205-aa41-5cc1c027cd14.png"> </p>

Balanced Random Forest Classifier
Accuracy Score: 0.79
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145718164-f68d59f5-adb8-4b67-9319-7914708f1137.png"> </p>

Easy Ensemble AdaBoost Classifier
Accuracy Score: 0.92
<p align="center"> <img src="https://user-images.githubusercontent.com/88862384/145718487-9ce7fb78-b2ac-4e85-bac2-9bebfd7285ce.png"> </p>

## Summary

In the situation of determing whether or not transactions are fraudulent, I believe recall is a stronger measure to rely on. I say this because although there are very low numbers of actual high risk transactions, if recall is high enough, there is a better chance of detecting fraud. From the images above we see that the models overall have low to satisfactory accuracy scores. Precision is very low amongst all of the models used. The only model with decent results used the Easy Ensemble alogorithm. This model had an accuracy score of 0.92 and recall of 91 and 94% for the high and low risk transactions, respectively. Although still low, its precision was highest among all models. I wouldn't recommend using any of these models because none have them provide reliable precision and the majority provide low accuracy scores and low recall.
