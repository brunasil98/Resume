                                            LoRa Proximity Model for Indoor Space

  This is my final project during Electronic and Electric Engineering Program at Norfolk State University. I completed it with my classmate Mrs. Alcaraz and our tutor, Dr. Guo. This was an application of LoRa technology. LoRa (short for long range) is a spread spectrum modulation technique derived from spread spectrum (CSS) technology developed by Semtech. LoRa devices enable IoT applications that solve the biggest current challenges in the world, such as energy management, pollution control, etc. It communicates through low power (928- MHz in the US) and enables long range transmissions up to 20 km (in open rural environments) and up to 2-3 km in urban environments with an outdoor gateway. This opens up a new world of possibilities of implementations to solve problems in rural and urban areas. Therefore, we decided to give our project a focus on the urban implementation side. 
  The goal of our project is to analysis the signal losses (Db power loss in our system) and create a model which could predict the distance between the gateway and end-node. Knowledge in wireless communication, Arduino software, microcontrollers and mathematics was required for the desired outcome. The model can be used to implement smart systems that provide important information to the user. Aa an example, a fire situation. The approximate localization of the fire can be tracked easily.
  
![image](https://user-images.githubusercontent.com/75848451/152470563-a9249107-9ed8-4a67-be20-d2fda14682b8.png)
  
  First, we set up a Server/Client network between the gateway and end-node to ensure that a two-way communication happens. Both equipment was setting up in the same frequency (868 MHz) via Arduino Software. After connected, they sent signals back and forward between each other, for collection of data. The end-node was assembled in each 2 meters of the apartment until got at 12 meters. 
  
![image](https://user-images.githubusercontent.com/75848451/152471446-9d7e0162-a00a-42af-a59a-9d70112a557c.png)

![image](https://user-images.githubusercontent.com/75848451/152471608-20d1e98a-e0d7-4a19-ac75-395d7cb1adf9.png)

  Due to environmental degradation we added procedures to give us more accuracy. First, we took a 10 point data set and removed the high and low outliers, and then averaged the remaining points to get a single point, and we repeated this procedure 10 times. After we got the full 10 points set, we also took out the high and low set with the 8 remaining points and plotted these points in a scatter graph. We created a Logistic Regression model using excel to find a relation between meters and signal loss. 
  
![image](https://user-images.githubusercontent.com/75848451/152471989-5b7da8f0-dbfb-4940-b408-7c9d9bd9815b.png)

  By looking at the results from the model developed it was clear that it was not 100% accurate. Therefore, it was necessary to perform an analysis to determine the error margin of the model. Data collection of the distance results from the model and the measured distance was done. To predict a better accountancy in our average and error margin, we also disregarded the high and low outlines. Thus, we calculated the Normalized Mean Square Root Error (NMSRE) to determine its accuracy and error probability. We found differences NMRSE, up to 0.125 in our model
  
![image](https://user-images.githubusercontent.com/75848451/152472106-4ae01d49-8cbd-4c6c-9987-4ba4ed65b477.png)

  It is crucial for its implementation and operation to consider the productivity and characterization of LoRa technology in indoor buildings. In this project, we have presented a comprehensive study how to utilize and predict LoRa in an indoor environment. It was a complete challenge to work in a project by using a new technology we had not utilized before. Looking at the results and after performing experiments testing the model, we realized that a perfect distance measurement is a tough task. When it comes to communication, it generally occurs in arbitrary conditions. This leads us to the fact that the model should be taken as a reference but not as a 100% accurate product. The findings presented in this paper can provide highlights into practical LoRa-based indoor applications.
