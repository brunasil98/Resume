# Convolutionla Network for Imperfection in a Sillicon Wafer

  In this project, I applied a CNN (Convolutional Neural Network) to detect errors in a silicon wafer, such as bubbles, extra material, extra extraction, and others. These errors affect the performance of the silicon wafer, which is an essential piece for manufacturing the semiconductors found in all kinds of electronic devices. My model can detect the imperfections before the wafer is used, saving a lot of time and effort from correcting a microchip made with a faulty wafer. The data set has 2688 images labeled either ‘error’ or ‘non-error’. I created a model with 21 layers and 2,011,429 parameters. The model has 3 convolution layers, 3 max pooling layers, 2 dropout layers, 5 batch normalization layers, 2 dense layers, and 1 flatten layer. 
  
   ![image](https://user-images.githubusercontent.com/75848451/152548004-46b090cd-0fc7-4d93-bbce-359328685e44.png)
   
The first steps of this application were transforming the image to black and white, dividing the pixels for 255 , splitting, and then normalizing the data set. To compile, I chose binary cross-entropy and RMSProp for loss and optimization, respectively. The model had batch size of 64, epochs of 1000, and validation split of 0.2.

   ![image](https://user-images.githubusercontent.com/75848451/152552497-b42cf543-c76b-42ee-8d34-63ab131ab9dd.png)
   
The model had an accuracy of 98.14% and a small number of false negatives, as you can see in the confusion matrix bellow. 

  ![image](https://user-images.githubusercontent.com/75848451/152553332-50eb50f5-4ac1-4bea-8564-a0d6169b5a41.png)
  
The model in general had good accuracy and effective results. However, the validation loss and accuracy had a lot of noise during the training. To further improve the model, next time I would choose a different normalization.
