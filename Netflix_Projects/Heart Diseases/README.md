                                            Predicting Heart Diseases In Medical Patients

  The dataset we chose was the Heart Disease dataset provided by UCI Machine Learning Repository. The dataset column to be tested will be the “target” column which will tested against the remaining columns to determine if we will be able to predict which patients will have heart diseases and if we are able to predict these cases. Through our different process methods, we hope to identify which will provide us the best results.
  
  This is our Data. The columns age and sex have the biggest correlation with the target (diseases or no diseases).

![image](https://user-images.githubusercontent.com/75848451/152437074-09b7a1eb-c9cf-49a1-be85-a364a3d4062a.png)

  The data has a bad distribution, while the first half of the rows was positive target, the other half was no target. 

![image](https://user-images.githubusercontent.com/75848451/152438399-da6810c5-dc60-495a-b4f8-e9220d152f1b.png)

  To the first model, we choose to build a Logistic Regression model using sklearn modulation. We split our data 80% as train the other 20% as test. To visualize our data, we plotted a confusion matrix, which compare the actual values and the predicted values of the model. The accuracy of this model was of 84%.

![image](https://user-images.githubusercontent.com/75848451/152438718-114648be-d098-4db9-90e9-cdf9e3374f42.png)

 Our Second model was a Random Forest Classifier. To train this data, we decided to balance the data set before. the model reduced the false negative which was our target due to the problem it can bring. The accuracy of this model was of 86,96%. 

![image](https://user-images.githubusercontent.com/75848451/152440373-bd3ffb30-b5f5-4640-bff8-8c40bd7e7f51.png)

 In this project, we created models to predict if the person has a heart diseases or not. We use two different approaches, one a linear regression, and second random forest classifier with balanced data. The second model has a better prediction and smaller error in false negative, which is crucial in biomedical field. The next steps would be the analysis of the false negative and try to find any relation between them. 
