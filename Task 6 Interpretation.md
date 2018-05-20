# Interpretation and Analysis

## Task 6: Spending v/s Table standing    

**Description**: There is a usual conception that more the spending a team does on it’s players the better is the result. We would like to observe how strong is the relation between the two in the League level table. 

**Method Used**: Correlation (both the variables are continuous) 

**Inputs**: 

 Correlation between:   Position & Spending
  
 Grouping by:           Year 
 
 Correlation Method:    Spearman Correlation (since, one of the variables is a numerical variable and other variable is a rank)

**Conclusion**:

•	There is a negative correlation between Position and Spending for all the years.

•	The average Spearman correlation observed for all the years combined is – 0.70. That means, as spending by team increases, the position decreases (i.e., …... 3,2,1).

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task6-Img1.png)

The correlation is – 0.70 which is although strong, but not strong enough as we expected. So, what happened? Why even when teams are spending so much on their players they could not end in top positions? 

The answer to this question is the bar graphs from SAS. From the bar graph, we observe that: The team who are with less spending end up with better position (or) team who are spending more not playing up to the standard. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task6-Img2-2.PNG)

This concludes that top 4 teams are dependent on the spending but are dependent on other factors i.e., their attack and defense. 

For example, we would like to consider the year 2015 – 2016 where the Spearman correlation between spending and position is the least (-0.52) and comment on the attack and defense for the teams. 

Leicester stood in position 1 for the year 2015 – 2016 although its spending was very less when compared to Manchester United with highest spending for that year standing 5th. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task6-Img3.png)

The above and below Tableau visualization we would like to use to better analyze the Defense and Attach respectively of the 10 top teams for 2015 – 2016. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task6-Img4.png)
  
  i.	Although the defense rate and keeper save accuracy for Man United is better when compared to Leicester, it is in the Attacking where Man United lacks. 

  ii.	The Man United’s attack especially their ability to shoot accurately i.e. shot accuracy is the scope of improvement and is a critical factor in them winning the match. 


