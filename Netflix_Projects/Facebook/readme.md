                      Dataset: We want to work with the facebook dataset from each of our individual profiles

Our Goal: We want to explore what statistic relates to the amount of likes, time a user has spent on the platform, and gender. We are trying to explore which of these areas is most likely going to influence whether and user will have increased traffic to their profile and postings. At the end of our research and after cleaning our dataset, we hope to prove whether or not time, age, or gender have an influence on your presense on facebook. 

**This information is solely based on Facebook's social media platform and not others such as Twitter,Instagram,TikTok,etc..


Current Questions to ask:
----
1. Which Generation Reacts more per hour?
2. Does the time you post effect the amount of likes ?
3. What type of post gets the most likes?
4. Which Gender sends the most friend request?
5. Which Gender rejects the most friend request?


Phase 1: Download individual datasets from FB -> https://www.facebook.com/dyi/?referrer=yfi_settings -> Likes_comments / Friends / Reactions
02/18/21
----
Phase 2: Work on cleaning data in alignment with question 02/23/21
----
 P1. (Create clean columns and remove null values)
      DataCleaning -> Facebook Plotlib.ipynb (jupyter notebook clean null values removed)
 
 P2. (Create dataframes of needed columns and remove excess data)
  
 P3. (Create statistical regression models if time)

Phase 3: Create plotly and matplotlib models 02/25/21
----  
 P1. Create mini subplots to display cross column data between dataframes
  
 P2. Establish labels and colors on data on plots

 P3 Transition plotly and matplotlib files to powerpoint presentation format (.jpg, .png)

Phase 4: Create Presentation outline and Review Visualizations (split 2:2) 03/02/21
----
 P1. Create framework/color schemes for data to be put into slide
 
 P2. Update transitions and icons/pictures to ensure they are properly formatted
 
 P3. Proof read for errors of spelling and slide transition timings.

Phase 5: Finalize presentation and Practice 03/02/21
----


CONCLUSIONS
1. Which Generation Reacts more per hour? 
   The engagement of younger generations is higher according to the amount of reactions. Surprisingly the hours of engagement do not variate between generations. The hours of activity are very similar and behave almost identically. 

2. Does the time you post effect the amount of likes?
   After reviewing the graph of reacitons against time of the day, it is very clear that the time that you post directly affects the amount of reactions that you might get. With a higher engagement between 1 pm - 3 pm and 10 pm - 1 am. These time slots representing the highest reactions received.
   
3. What type of post gets the most likes?
   After analysisng the scatter graph of posts vs reactions it was very clear that the 'Post' type were the ones getting the most reactions. This category corresponds to status updates of the user. Also, the time that these post were made was affecting directly on the amount of reactions it would get. We can see that the amount of reactions drops significantly when is not at the key hours (1 pm - 3 pm and 10 pm - 1 am).
   
4. Which Gender sends the most friend request?
   Surprisingly the Female Group showed to be the one to have the most friend request sent. We were expecting the opposite before coming up to the result.
   
5. Which Gender rejects the most friend request?
   The Female Group ended up being the one that rejects the most friend requests as well. With a very long difference compared to the Male Group. This could also be  caused because the possibility of receiving more friends requests compared to Male. That would be a factor to consider for future analysis on the subject
