                                                LoRa Proximity Model for Indoor Space

  This was my final project for my Electronic and Electric Engineering Program at Norfolk State University. I completed it with my classmate, Ms. Alcaraz, and our advisor, Dr. Guo. LoRa (short for long range) is a spread spectrum modulation technique derived from chirp spread spectrum (CSS) technology developed by Semtech. LoRa devices enable Internet of Things (IoT) applications that solve the biggest current challenges in the world, such as energy management, pollution control, etc. It communicates through low power (928 MHz in the US) and enables long range transmissions up to 20 km (in open rural environments) and up to 2-3 km in urban environments with an outdoor gateway. This opens up a new world of possibilities to solve problems in rural and urban areas. Therefore, we decided to give our project a focus on the urban implementation side. 
The goal of our project was to analyze the signal losses (dB power loss in our system) and create a model which could predict the distance between the gateway and end-node. Knowledge in wireless communication, Arduino software, microcontrollers, and mathematics was required for the desired outcome. The model can be used to implement smart systems that provide important information to the user. For example, in the event of a large fire, responders could easily transmit information throughout the area.

![image](https://user-images.githubusercontent.com/75848451/152470563-a9249107-9ed8-4a67-be20-d2fda14682b8.png)

First, we set up a Server/Client network between the gateway and end-node to facilitate two-way communication. All equipment was set up at the same frequency (868 MHz) via Arduino Software. After connected, they sent signals back and forth between them, which was how we collected data. The end-node was incrementally moved 2 meters further from the gateway until it was 12 meters away. 

![image](https://user-images.githubusercontent.com/75848451/152471446-9d7e0162-a00a-42af-a59a-9d70112a557c.png)
![image](https://user-images.githubusercontent.com/75848451/152471608-20d1e98a-e0d7-4a19-ac75-395d7cb1adf9.png)

  Due to environmental degradation, we added steps to give us more accuracy. First, we took a 10-point data set and removed the high and low outliers, and then averaged the remaining points to get a single point, and we repeated this procedure 10 times. After we got the full 10-point set, we also took out the high and low set with the 8 remaining points and plotted these points in a scatter graph. We created a Logistic Regression model using excel to find a relation between meters and signal loss.
  
![image](https://user-images.githubusercontent.com/75848451/152471989-5b7da8f0-dbfb-4940-b408-7c9d9bd9815b.png)

By looking at the results from the model it was clear that it was not 100% accurate. Therefore, it was necessary to perform an analysis to determine the error margin of the model. To predict a better accountancy in our average and error margin , we also disregarded the high and low outlines. Thus, we calculated the Normalized Mean Square Root Error (NMSRE) to determine its accuracy and error probability. We found different NMRSEs in our model, up to 0.125.

![image](https://user-images.githubusercontent.com/75848451/152472106-4ae01d49-8cbd-4c6c-9987-4ba4ed65b477.png)

It is crucial for its implementation consider the characteristics of LoRa technology in indoor buildings . In this project, we presented a comprehensive study on how to utilize and predict LoRa in an indoor environment. It was a challenge to work with a new technology we had not utilized before. Looking at the results and after testing the model, we realized that it is a tough task to measure distance accurately. However, with respect to wireless communications, distance typically does not need to be totally exact. This leads us to conclude that the model should be taken as a reference but not as a 100% accurate product. The findings presented in this paper can provide highlights into practical LoRa-based indoor applications.
