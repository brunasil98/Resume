                                            Predicting Heart Diseases In Medical Patients

  The dataset we chose was the Heart Disease dataset provided by UCI Machine Learning Repository. The dataset column to be tested will be the “target” column which will tested against the remaining columns to determine if we will be able to predict which patients will have heart diseases and if we are able to predict these cases. Through our different process methods, we hope to identify which will provide us the best results.
  
  This is how the data set looks. The columns age and sex have the biggest correlation with the target (diseases or no diseases).

![image](https://user-images.githubusercontent.com/75848451/152437074-09b7a1eb-c9cf-49a1-be85-a364a3d4062a.png)

  The data has a bad distribution, while the first half of the rows was positive diseases, the other half was no diseases. 

![image](https://user-images.githubusercontent.com/75848451/152438399-da6810c5-dc60-495a-b4f8-e9220d152f1b.png)

  For this first model, we chose to build a Logistic Regression model using sklearn modulation. We split our data 80% as train the other 20% as test. To visualize better the results, we plotted a confusion matrix, which compares the actual values and the predicted values of the model. The accuracy of this model was 84%. The performance was better than what we expected, the high accuracy and low false negative for a Logistic Regression without modulated the data, was surprising.  

![image](https://user-images.githubusercontent.com/75848451/152655026-5e57d4ba-7d40-4cbc-bee0-a074e56f459b.png)

 In our Second model was a Random Forest Classifier. To train this model, we decided to balance the data set. the model reduced the false negative which was our target due to the problem it can bring. The accuracy of this model was 86,96%. The model achived its goal, which was decreasing the false negative from 0.19 to only 0.086 error.

![image](https://user-images.githubusercontent.com/75848451/152655021-12069f71-9784-418e-b09a-dcacd0c0d4fc.png)

 In this project, we created models to predict if the person has a heart diseases or not. We used two different approaches, one a linear regression, and second random forest classifier with balanced data. The second model has a better prediction and smaller error in false negative, which is crucial in biomedical field. The next steps would be the analysis of the false negative and try to find any relation between them. 
