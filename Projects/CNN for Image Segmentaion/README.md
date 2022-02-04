# U-Net: Convolutional Network for Image Segmentation

  This implementation was a convolutional neural networks application, which has the ability to label to each pixel of an image. This was created by Olaf Ronneberger, Philipp Fischer, and Thomas Brox at University of Freiburg. This was a breakthrough in image segmentation, as it gives a label for each pixel through a extend convolutional network which is known as U-Net. The implementation is very important for the biomedical field. The application applied a network to cells in order to find the precise edge of a cell. Hence, the cell can be easily measured, and, according to how it stretches, one can determine if the cell is cancerous or not. 

  The main idea of this application was to decrease the number of pixels while at the same time increasing the number of filters, until the image is 32x32 pixels and has had 1024 filters applied. Next, the model starts to return to the number of pixels and filters of the original image, in this case 512x512 and 1 filter. The shape of the model is similar to the letter ‘U’, hence the name U-Net
  
 ![image](https://user-images.githubusercontent.com/75848451/152475561-8b1f7f5b-ba73-4adb-99db-953bd7efc9b0.png)

  TThe data was obtained through Dr. Deo’s research. However, the images are low quality and blurry as you can see in the first picture. Thus, it became a big challenge to measure the diameter size of the cells. Due to the research consists of finding a cancer diagnostic through cells diameter.

 ![image](https://user-images.githubusercontent.com/75848451/152476190-5945cdf6-f24b-42a4-8e31-f88b4e1b2c9a.png)

  Another important aspect of this operation was the employment of data augmentation, implemented by applying elastic deformations to the 30 and 51 available training images to create additional images. This is particularly important in biomedicine both because of the aforementioned scarcity of available pictures as well as the resulting accuracy, since it is able to efficiently simulate deformation, which is a common variation in tissue. The model was trained using 100 epochs each containing 10 images, generating a total of 1000 images. Increasing the number of images in each epoch did not lead to better results, likely due to the model overfitting the images because of the data augmentation. 
  
 ![image](https://user-images.githubusercontent.com/75848451/152476293-da47153a-e8af-4dfd-b0f2-d65fb81237c2.png)

  It is clear that more data is needed for the model to perform as expected. Analyzing the images above, the model with 51 images clearly outperforms the model with 30 images. The model with 51 images started to identify other anomalies around the cell as well. 
  
  This project produced a model similar to one presented in U-Net: Convolutional Networks for Biomedical Image Segmentation by Olaf Ronneberger, Philipp Fischer, and Thomas Brox. The images utilized were provided by Dr. Deo’s research at Norfolk State University about how cells stretch under specific conditions. However, the pictures acquired did not have high enough quality to be able determine the location of the edge exactly. Therefore, it requires image segmentation just as many biomedical images do. 
