# Convolutionla Network for Imperfection in a Sillicon Wafer

  In this project I did a implementation of a CNN (Convolutional Neural Network) in a selicon wafer to detect bubles, extra material, extra extraction and others, which affects the performaces of a semi-conductor. A silicon wafer is a material essential for manufacturing semiconductors, which are found in all kinds of electronic devices that are in our lives. With this implemetaion, the manuffecture can detect the imperfections before the performance, consequently, it decreases the time spent and money in each device. The data set has 2688 images and in each image has a label with error or non eroor.
  
   For this implementation I use a CNN model for image classification. I created a model with 21 layers and 2011429 parameters. The model had 3 convotuion layer, 3 max pooling layer, 2 droupout layer, 5 batchnormalization layer, 2 dense layer and 1 flaten layer. 

![image](https://user-images.githubusercontent.com/75848451/152548004-46b090cd-0fc7-4d93-bbce-359328685e44.png)

  The first step of this implementation was transforming the image in black and white, dividing the pixes for 255, split and than normalize the data set. The compile, I have choose a binary crossentropy and rmsprop for loss and optimizer respectively. The model had batch size of 64, epochs of 1000 and validation split of 0,2.
  
  ![image](https://user-images.githubusercontent.com/75848451/152552497-b42cf543-c76b-42ee-8d34-63ab131ab9dd.png)

  The model has a accurancy of 98,14% and smaller number of false negative, as you can see in the confusion matrix bellow. 
  ![image](https://user-images.githubusercontent.com/75848451/152553332-50eb50f5-4ac1-4bea-8564-a0d6169b5a41.png)

  The model in geral had a good accurancy and effect results. The validation loss and and accuracy has a tremoous noise when were train which is the lowest point of the model. For the next steps that would be the priority as chose a diferent normalization of vizualize the data had not predict correct. 
