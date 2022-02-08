# U-Net: Convolutional Network for Image Segmentation


For this project, I used a convolutional neural network (CNN) model with the ability to label each pixel of an image. This was created by Olaf Ronneberger, Philipp Fischer, and Thomas Brox at the University of Freiburg. This was a breakthrough in image segmentation, as it gives a label for each pixel through an extended convolutional network which is known as U-Net. This implementation is very important for the biomedical field. This project applied a U-Net to images of cells in order to find the precise edge of a cell. This allows the cell to be easily measured so that one can determine whether the cell is cancerous or not according to how it stretches.
The main idea of this project was to decrease the number of pixels while at the same time increasing the number of filters, until the image is 32x32 pixels and has had 1024 filters applied. Next, the model starts to return to the number of pixels and filters of the original image, in this case 512x512 and 1 filter. The shape of the model is similar to the letter ‘U,’ hence the name U-Net

 ![image](https://user-images.githubusercontent.com/75848451/152475561-8b1f7f5b-ba73-4adb-99db-953bd7efc9b0.png)
 
The images were obtained from the research of Dr. Makarand Deo at Norfolk State University, which consists of diagnosing cancer by measuring cells' diameters. However, the images are low quality and blurry, as seen in the first picture, making it challenging to measure the diameter of the cells. In order to help overcome this challenge, this project develops a mask for each image to highlight the cells, as seen in the second and third pictures here: 

 ![image](https://user-images.githubusercontent.com/75848451/152476190-5945cdf6-f24b-42a4-8e31-f88b4e1b2c9a.png)
 
Another important aspect of this project was the use of data augmentation, implemented by applying elastic deformations to the available training images to create additional images. This is particularly important in biomedicine because of both the scarcity of available pictures as well as the resulting accuracy, since it is possible to easily simulate deformation, which is a common variation in tissue. The model was trained using 100 epochs each containing 10 images, generating a total of 1000 images. Increasing the number of images in each epoch did not lead to better results, likely due to the model overfitting the images because of the data augmentation. 

 ![image](https://user-images.githubusercontent.com/75848451/152476293-da47153a-e8af-4dfd-b0f2-d65fb81237c2.png)
 
It is clear that more data is needed for the model to perform as expected. Analyzing the images above, the model with 51 images clearly outperforms the model with 30 images. The model with 51 images started to identify other anomalies around the cell as well. However, the pictures acquired did not have high enough quality to be able to determine the location of the edge exactly. 
