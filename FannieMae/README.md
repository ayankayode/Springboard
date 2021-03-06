# Predicting mortgages prone to foreclosure during economic recession

The 2008 recession was an eye-opener for the government of many countries, organizations, industries and individuals. One of the common occurrences during periods of recession is that some mortgage loans that were not at risk of default in a normal economy become susceptible to foreclosures due to significant changes in financial status of borrowers. This means that the normal risk analysis models may not necessarily identify borrowers that will default during adverse economic situations. Previous studies indicate that the number of foreclosures could be more than double of the normal rate of foreclosures in a stable economy. Therefore, it is important to lenders to be able to identify the characteristics of mortgages on their books that are at risk of foreclosures in case of another economic recession.

## Major Questions

1. What are the characteristics of mortgages at the risk of foreclosure during economic recession and during the initial recovery period, typically 12 months after the last month of economic decline.
2. How far backwards or close to a recession can mortgages at risk of recession be detected?
3. To what degree of accuracy can we predict a mortgage at risk of foreclosure, in case of recession.

## Data
Fannie Mae, a government-sponsored enterprise that offers different types of mortgage loans provides open access to Single Family Mortgage dataset that was used for this study. The dataset consists of nearly 22 million records with a static acquisition file and a one to many monthly performance loan-level details for each quarter of the year since inception. Using the 2008 recession as the reference point, the period of 01 January 2008 and 31 December 2010 is considered as the recession and recovery period. Thus, only mortgages foreclosed during this period were considered as affected by the recession. 

## Methodology
Logistic regression and XGBoost techniques were explored - XGBoost had better results.

## Result
Different experiments were carried out using Support Vector Machines(SVM), Logistic Regression and Gradient Boosting (XGBoost). XGBoost had the best result in predicting which loan will or will not foreclose during a recession with a weighted 97.86% accuracy. Specifically, 73% accuracy was achieved in identifying loans that are prone to foreclose depending mainly . 

Overall, the results show that mortgage with low equity to value ratio that the property is based in California, Florida or Arizona that has never been modified (improved/extended) are more prone to foreclosure during a recession that the others Other important factors that makes a mortgage prone to foreclosure in recession are If it is not a primary residential property, the original term is above average and the debt to income ratio of the borrower is in the upper limit of what is acceptable.

Finally, the distribution of the confusion matrix per year show that predictions are more accurate as we move closer to the year of recession.


## Author
Kayode Ayankoya
