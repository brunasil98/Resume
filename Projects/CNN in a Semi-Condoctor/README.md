# Convolutionla Network for Imperfection in a Sillicon Wafer

  In this project I did an application of a CNN (Convolutional Neural Network) in a silicon wafer to detect any error as bubbles, extra material, extra extraction, and others. These errors affect the performance of a silicon wafer. A silicon wafer is a material essential for manufacturing semiconductors, which are found in all kinds of electronic devices that are in our lives. With this performance, the model can detect the imperfections before install the product in the hardware, consequently, it saves a lot of time and problems. The data set has 2688 images and, in each image has label (error or non-error).
     I created a model with 21 layers and 2011429 parameters. The model has 3 convolution layer, 3 max pooling layer, 2 dropout layer, 5 batch normalization layer, 2 dense layer and 1 flatten layer. 

   ![image](https://user-images.githubusercontent.com/75848451/152548004-46b090cd-0fc7-4d93-bbce-359328685e44.png)

  The first steps of this application were transforming the image in black and white, dividing the pixels for 255, split and then normalize the data set. The compile, I have chosen a binary crossentropy and rmsprop for loss and optimizer respectively. The model had batch size of 64, epochs of 1000 and validation split of 0,2.
  
   ![image](https://user-images.githubusercontent.com/75848451/152552497-b42cf543-c76b-42ee-8d34-63ab131ab9dd.png)

  The model has an accuracy of 98,14% and smaller number of false negative, as you can see in the confusion matrix bellow. 
  
  ![image](https://user-images.githubusercontent.com/75848451/152553332-50eb50f5-4ac1-4bea-8564-a0d6169b5a41.png)
  
  The model in general had a good accuracy and effective results. The validation loss and accuracy during the training had a tremulous noise, this was the lowest point of the model. For the next steps that would be the priority, chose a different normalization.


