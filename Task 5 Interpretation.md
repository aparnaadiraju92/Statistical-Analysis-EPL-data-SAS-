# Interpretation and Analysis

## Task 5: How Betting odds are impacting a match    

**Description**: In Europe, betting is considered legal. Betting odds are established, and bets are taken by companies like Betting365 (B365 in our data). B365 odds are basically Home team winning odds (B365H), Away team winning odds (B365A), match draw odds(B365D). (B365D), are always somewhere b/w (B365H), (B365A). The minimum off the odds is the result of B365. Suppose for example:

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task5-Img1.PNG)

We have considered betting odds provided by B365 to verify if:

i.	Actual full-time results and B365 results are dependent. 

ii.	Observe the moderation effect of B365results on the relationship between Full-Time Goal Difference and Half-Time Goal Difference. 

**Test 1: Actual full-time results and B65 results are dependent**

**Null Hypothesis**: Variables are independent.  

**Alternate Hypothesis**: Variables are dependent. 


**Method Used**: Chi Square test for Independence (since both the variables are categorical)

**Inputs**: 

 Row Variable:  B365RESULT (H = Home, A = Away)
  
 Column Variable: FTR (Full Time Result: H = Home, D = Draw, A = Away


**Output and Inferences**:

•	From the table, we can observe that the model is significant as the Chi-Square p value is less than alpha. 

•	Chi-square value is 207.8031 which is high.

•	Phi Coefficient is 0.3697 which is interpreted as correlation. Correlation positive and not so strong. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task5-Img2.png)


**Conclusion**:

From the Table analysis graph, we can see that:

•	B365Results are favorable to Home team win

•	If the B365 result is Away win, the Away team winning the match is high compared to the match being a draw or home team win. 

•	If the B365 result is Home win, the Home team winning match is high compared to Away team winning or match being draw. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task5-Img3.png)

**Test 2: Observe the moderation effect of B365results on relationship b/w Full-Time Goal Difference and Half-Time Goal Difference.**

**Null Hypothesis**: There is no interaction effect.  

**Alternate Hypothesis**: There is an interaction effect. 


**Method Used**: Multi linear regression (since, the dependent variable is numerical continuous)

**Inputs**: 

 Dependent Variable:  FTGD (Full Time Goal Difference)
  
 Independent Variable:  Continuous: HTGD (Half Time Goal Difference) 
		        Categorical: B365result (H = Home, A = Away)

**Interaction**: HTGD * B365

**Output and Inferences**:

•	From the ANOVA table, the value of F statistic is very high 603.22. The p value is <0.001 which is less than alpha. This implies model is significant. 

•	54.32% of total variance of dependent variable is explained by the independent variables. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task5-Img4.png)

**Conclusion**:

From the parameter estimates table, the parameter estimates columns are the measure of change in Y, for one-unit change in X. 

Considering the variables for which p is less than alpha, the significant variables are:  **HTGD, B365RESULTA** 

However, HTGD * B365RESULTA is not a significant factor and that implies there is no interaction effect. 

![alt text](https://github.com/mullapudirajaprashanth/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task5-Img5.png)
