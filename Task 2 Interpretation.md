# Interpretation and Analysis

## Task 2: Clustering the referees into 2 - Harsh referee and Lenient referee   

**Description**: In a football match, if any player performs an action which he is not supposed to do as per the game rules, 
a referee will give the player a foul (first warning), a yellow card (final warning) and red card (serious offense, action taken) 
depending upon the level of severity of the incident. By considering the fouls committed by the team to the booking points given 
by the referee we would like to cluster the referees who were part of *more than 10 matches* into Harsh and Lenient. 

	Booking points = Number of Yellow cards * 10 + Number of Red cards * 25
 
**Method Used**: K means clustering (since, we already know how many clusters we want for our analysis)

**Inputs**: 

 Filter:  Numberofmatches > 10
  
 Clustering based on the variables:- Continuous: AVGHOMEFOULS, AVGAWAYFOULS, AVGHOMEBP, AVGAWAYBP

**Code used**:

We have written an SQL query to get the desired variable grouped by Referees. The sample of output table data looks like:

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task2-Img1.png)


**Output and Inferences**:

•	The cluster summary table states that, there 7 referees who come under cluster 1 and 14 referees who are under cluster 2. 
Cluster 1 is close to cluster 2 and vice-versa. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task2-Img2.png)

•	The cluster listing table clearly identifies the observations and the cluster to which the observation belongs to. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task2-Img3.png)


**Conclusion**:

The characteristic of cluster means for each cluster are observed and we concluded that,

•	Cluster 1 – Lenient referees

•	Cluster 2 – Harsh referees

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task2-Img4.png)

Lenient referees give away less fouls and booking points in matches when compared to Harsh referees who tend to consider every minute mistake. 
We found that this general characteristic of referees tends to remain same in almost 85% matches. 
