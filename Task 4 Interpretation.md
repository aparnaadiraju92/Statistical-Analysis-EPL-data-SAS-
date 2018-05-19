# Interpretation and Analysis

## Task 4: Established Rivalries (Derbies) and match results         

**Description**: Established Derby Rivalries between intra-city teams brings the best out of teams, and we would like to know 
how well they play during their derby matches, non-derby matches and compare it with all other matches played by non-derby teams. 
Below are some of the established derby rivalries which were analyzed in our test: 
 
•	Manchester United v/s Manchester City
•	Arsenal v/s Tottenham
•	Chelsea v/s Arsenal
•	Liverpool v/s Everton

**Example of a type of match**:

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task4-Img1.PNG)

**Null Hypothesis**: The Type of match (Derby / Non-Derby) does not play any significant factor in the Full-time Result of the match.

**Alternate Hypothesis**: The Type of match (Derby / Non-Derby) should play as a significant factor in the Full-time Result of the match.


**Method Used**: Chi Square test for Independence (since both the variables are categorical)

**Inputs**: 

 Row Variable:  FTR (Full Time Result : H = Home, D = Draw, A = Away)
  
 Column Variable: 
    
    TypeofMatch (0,1,2,3) 
    0 = Derby team Home v/s Derby Team Away                1 = Derby team as Home v/s Non-Derby team as Away
    2 = Non-Derby team as Home v/s Derby team as Away      3 = Non-Derby team v/s Non-Derby Team


**Output and Inferences**:

•	From the table, we can observe that the model is significant as the Chi-Square p value is less than alpha. 

•	Chi-square value is 158.29 which is high.

•	Phi Coefficient is 0.3227 which is interpreted as correlation. Correlation positive and not so strong. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task4-Img2.png)


**Conclusion**:

From the Table analysis graph, we can see that:

•	There are few derby matches held overall compared to other types of matches

•	0 - During a Derby match, i.e. Derby Home team vs Derby Away team; The Derby Team playing at Home either wins or draws most of the matches. Derby team playing at home will rarely loose a match to its Derby rival at Home.

•	1 - During a Normal match where a Derby playing team is at Home vs a non-Derby playing team as Away team; the Derby Team performs much better in these matches and have higher win%.

•	2 – During a Normal match were a non-Derby team is at home and Derby playing team is an Away team; the Derby playing team performs much better and have higher win%.

•	3 – During a Normal match played between non-Derby teams; the chances of the team playing at home to loss a match is less compared to the away team winning or drawing the result. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task4-Img3.png)
