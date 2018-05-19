# Final Report
## Interpretation and Analysis

### Task 1: Identify the factors which will predict the Final match result.

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

Output and Inferences:

•	The generalized logit model and Newton-Raphson optimization technique are considered in a Multi-nominal logistic regression. 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img2.png)

•	The reference category to be considered is FTR = ‘H’ 

![alt text](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Output%20Images/Task1-Img3.png)
