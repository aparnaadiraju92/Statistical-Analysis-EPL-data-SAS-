# Interpretation and Analysis

## Task 1: Identify the factors which will predict the Final match result.

**Description**: Each and every factor recorded in our Match level data set at some point would have helped in changing the match result. Through this question, we want to observe what factors predict the Final match result when all these are considered together. 

**Null Hypothesis**: No factor plays a role in predicting Final match result. 

**Alternate Hypothesis**: We expect at least one factor to play a role in predicting the Final match result. 


**Method used**: Multi nominal logistic regression (since, dependent variable is categorical with 3 categories)


**Inputs**: 

  **Dependent variables**:  FTR (event = ‘H’)
  
  **Independent variable**: 
                            Categorical: HTR
                            Continuous: HS, AS, HST, AST, HC, AC, HF, AF, HY, AY, HR, AR

Code used:

Since, SAS does not allow us to perform **Multi-Nominal Logistic Regression**  test by default, we have written a SAS code by customizing the existing Binary Logistic Regression Code. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img1.png)

**Output and Inferences**:

•	The generalized logit model and Newton-Raphson optimization technique are considered in a Multi-nominal logistic regression. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img2.png)

•	The reference category to be considered is FTR = ‘H’ 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img3.png)

•	The -2 Log L value of fitted model (2201.339) is less than the value of -2 Log L value for Null model (3227.332). The fitted model is considered to be better. 

•	55.75% of variance of dependent variables is explained by the independent variables taken.

•	As the p value (<0.001) from the likelihood ratio is less than alpha, Model is significant and at least one factor is playing a role in predicting the Final match result. 

•	From the Maximum Likelihood estimates table, the parameter estimates columns in this table is the measure of log odds for Y = A (or) D with relative to Y = H for one-unit change in X. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img4.png)

**Conclusion**:

Considering the variables for which p is less than alpha, 

The significant variables for log odds of dependent variable Y = A relative to Y = H are: 
 
                                                                                     HTR, HST, AST, HC, AC, HR, AR

The significant variables for log odds of dependent variable Y = D relative to Y = H are: 
 
                                                                                     HTR, HST, AST, HC, AC, AR

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img5.png)
