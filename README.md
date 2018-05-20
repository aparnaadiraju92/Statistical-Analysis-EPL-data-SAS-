# Statistical Analysis on EPL data
  We will be using SAS (University Edition), Excel, and Tableau for this analysis. 

## INTRODUCTION

#### Objective

The main purpose of the project is to perform Analysis on a specific set of data mainly using the Statistical methods and provide inferences from the results obtained. 

#### Executive Summary

This report summarizes the statistical modeling and analysis results associated with English Premier League. The purpose of this report is to document implemented sampling design and all corresponding data modeling and inference techniques used during our statistical analysis.
English Premium League EPL is a professional league for men’s association football clubs. The primary role of the English Premier League is to organize the football competition between the 20 Clubs that make up the league. In revenue terms, it is now the third largest league in the world, behind the US Major League Baseball and National Football League (American Football). 

The data for our analysis has been derived from two sources  – ‘The official EPL website’ and ‘EPL Stats blog’.

#### Data Description

The main reason for choosing this data set is, the Premier League is the most-watched sports league in the world and we felt it would be interesting to do a statistical analysis on this data. 

The Dataset used for the performing the analysis is a comprehensive data set which contains the details of each match EPL (Match level) has hosted for the years between 2013-2017. The data for each year (2013-2014, 2014-2015, 2015-2016, 2016-2017) is downloaded from the data source mentioned below and downloaded files are merged to form a single file for better analysis. Also, we are using EPL dataset at Season level for the same years which is giving us the Table standings of Teams and summary for each team for that year with their spending. 

Initial source of Data - http://www.football-data.co.uk/englandm.php and http://www.footstats.co.uk/index.cfm?task=league_full

The raw datasets are available in the named [Initial Datasets](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/tree/master/Initial%20Datasets)

#### Data Exploration
Apart from cleaning and normalizing the data we have performed feature engineering at several levels of data to make sure our analysis provides a valuable insight. (example feature: ‘Booking Points’ which is actually derived from valuating the  yellow, red cards and other fouls which in turn play a vital role in match result. This feature helps SAS to identify the significance and severity of an offence).

The clean datasets used for analysis are readily provided in this repository.
1. Match Level data for 4 seasons [here](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/ProjectMatchleveldata_R.xlsx)
   
2. League Level data for 4 seasons [here](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/ProjectLeagueleveldata.xlsx)

The Key to variable names is available in the file named [Data Key](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Data%20Key)

## Analysis tasks:

The analyses will help everyone to have a deeper insight on match level and league level statistics. Our Analysis include several interesting tasks like: 
                                 
#### 1. ####	
Identify the factors which will predict the Final match result. [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%201%20Interpretation.md)

#### 2. ####
Clustering the referees into Harsh referee and Lenient referee based on the Fouls committed by the teams and Booking Points given by the referee in the matches over the seasons. [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%202%20Interpretation.md)

#### 3. ####
Does the type of Referee (clustered in the above task) play a role in predicting the Final match result? [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%203%20Interpretation.md)

#### 4. ####
Analyze if Full Time match result and type of match are dependent. Identifying the established sport rivalries and analyzing results from the derby matches and the matches played by the derby teams against other teams as Home and as Away.  [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%204%20Interpretation.md)

#### 5. ####
Analyzing if Betting result and Full-Time match result are dependent. Observe if there is any moderation effect on the relationship between Full-Time Goal Difference and Half-Time Goal Difference. [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%205%20Interpretation.md)

#### 6. ####
Identifying how the Spending (i.e., Player wages) by each team impact Table standings each season. Does a team that spends more money on its players end up qualifying for Champions League i.e., being in the top 4 teams list on the league table? [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%206%20Interpretation.md)


## Analysis - Interpretation - Conclusion:

From the analysis performed on the questions we set up at the start of the project, following are the conclusions drawn from the analysis we have performed:

•	Significant variables in predicting final match result: HTR, HST, AST, HC, AC, HR, AR [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%201%20Interpretation.md)                                     

•	Referees clustered to Lenient referee and Harsh referee [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%202%20Interpretation.md)

•	Type of referee not a significant factor in predicting match result [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%203%20Interpretation.md)

•	Derby teams have less chance in losing match at Home [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%204%20Interpretation.md)

•	Betting odds favorable to Home team win [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%205%20Interpretation.md)

•	Half Time Goal Difference and Betting results significant in determining Full Time Goal Difference [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%205%20Interpretation.md)

•	Average correlation between Position and Spending is -0.70 [Interpretation](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/Task%206%20Interpretation.md)


## SAS Codes ##
The codes are available in the .md file [EPL codes](https://github.com/aparnaadiraju92/Statistical-Analysis-EPL-data/blob/master/EPL%20codes.sas7bdat)


