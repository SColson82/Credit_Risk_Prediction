# Supervised Machine Learning Challenge: Predicting Credit Risk
<hr>

Using machine learning models, this challenge was to attempt an assessment at whether a loan from LendingClub will become high risk or not. 

Models used:

* Logistic Regression
* Random Forest Classifier


## Process:

The test set was undersampled data from 2019 which consisted of 50-50 split of low and high-risk data. This was converted from categorical to numeric data and used to train both models using both unscaled data and data scaled using the StandardScaler function. Therefore, we were left with four trained models. These were then tested using undersampled data (again converted from categorical to numeric data) consisting of a 50-50 split of high and low risk data from the first quarter of 2020. 


## Theory:

My theory was that the Random Forest Classifier-Scaled model would perform best of all four models followed by Random Forest Classifier-Unscaled, Logistic Regression-Scaled, and finally by Logistic Regression-Unscaled. I assumed that scaling the data would improve both the Logistic Regression and the Random Forest Classifier but based on my understanding that more weight is given to some features than others when Random Forest is applied I assumed that it would outperform Logistic Regression which applies equal weight to each feature and can lose accuracy with high amounts of categorical data and with increase in 'noise'.

## Conclusion:  

I was incorrect. The model that proved the most accurate was Logistic Regression-Scaled followed by Random Forest both scaled and unscaled which were both the same level of accuracy across the testing set and then Logistic Regression-Unscaled. It is worth noting that there was 1.00 accuracy on the testing set for Random Forest-Scaled but accuracy fell to 0.623 across the testing set, which might indicate that the model was overfitted. One thing I might try for this would be to increase the training data and try again. 

✅ As for the winner, Logistic Regression-Scaled scored a 0.760 accuracy for the testing data. In a professional setting, this accuracy score might indicate a need for further review and possible implementation. 


![image](https://user-images.githubusercontent.com/83737584/140003154-041fa09f-256a-404d-8d74-f5420d370876.png)


