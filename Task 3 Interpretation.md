# Interpretation and Analysis

## Task 3: Does the type of Referee play a role in predicting the Final match result ?     

**Description**: With the significant factors we got from Task 1, we added the Type of Referee variable 
(cluster 1 or 2 from previous Task 2) to see if it is a significant factor in predicting the match result.

**Null Hypothesis**: Type of Referee does not play a role in predicting the Final match result. 

**Alternate Hypothesis**: Type of Referee does play a role in predicting the Final match result. 


**Method Used**: Multi nominal logistic regression (since, dependent variable is categorical with 3 categories)

**Inputs**: 

 Dependent Variable:  FTR (event = ‘H’)
  
 Independent Variable: 
    
    > Categorical: HTR, Referee_Cluster
    
    > Continuous: HST, AST, HC, AC, HR, AR

**Code used**:

Since, SAS does not allow us to perform Multi-Nominal Logistic Regression test by default, 
we have written a SAS code by customizing the existing Binary Logistic Regression Code. 


**Output and Inferences**:

•	The generalized logit model and Newton-Raphson optimization technique are considered in a Multi-nominal logistic regression.  

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task3-Img1.png)

•	The reference category to be considered is FTR = ‘H’ 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task3-Img2.png)

•	The -2 Log L value of fitted model (2212.068) is less than the value of -2 Log L value for Null model (3215.012). 
The fitted model is considered to be better. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task3-Img3.png)

•	55.02% of variance of dependent variables is explained by the independent variables taken.

•	As the p value (<0.001) from the likelihood ratio is less than alpha, model is significant. 

•	From the Maximum Likelihood estimates table, the parameter estimates columns in this table is the measure of log odds 
for Y = A (or) D with relative to Y = H for one-unit change in X. 


**Conclusion**:

Considering the variables for which p is less than alpha, 
The significant variables for log odds of dependent variable Y = A relative to Y = H are: 
    
    > HTR, HST, AST, HC, AC, HR, AR

The significant variables for log odds of dependent variable Y = D relative to Y = H are: 
    
    > HTR, HST, AST, HC, AC, AR

The Referee_cluster is not a significant factor in predicting the Final result of match as the value of p is greater than alpha.

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task3-Img4.png)
