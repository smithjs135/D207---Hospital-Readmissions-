# Hospital Data: Project Overview 
______________________________________________________________________________________________________________________________________________________________________
* Created a tool that cleans and explores hospital data

## Research Question
Can hospital patient readmissions be predicted based on the services received at the hospital during his or her initial visit? Are there additional indicators (variables) of hospital readmissions that may prove useful?

## Stakeholder Benefit
Hospital executives are under increased scrutiny when patients have unplanned readmissions within 30 days after the initial visit. The Centers for Medicare and Medicaid Services (CMS), under the Hospitals Readmissions Reductions Program, may withhold regular reimbursements for excessive 30-day readmissions for select diagnoses (Saunders, 2012, Introduction). Stakeholders can implement steps to reduce hospital readmission rates if they know which patients are most likely to be readmitted and if they know which factors potentially lead to readmissions.

##  B3. Justification:
The chi2_contingency test was selected for its suitability to work with categorical variables. In addition, the chi2_contingency test can be used with skewed data so long as the sample size is sufficiently large (MchHugh (Jun, 2013, Section: Introduction).  The data set contains 9,999 rows which is sufficiently large for this analysis.  See python output (B2).
“ReAdmis” is the dependent variable, a binomial and is necessary to answer the question “Can we predict when a patient is likely to be readmitted? “. 


## Code and Resources Used
**Python Version:  ** Python version: 3.8.5
**Packages:** pandas, numpy, scipy, seaborn, matplotlib
## EDA
Visualizations including boxplots and a heatmap:

![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_ReAdmis-Initial_days.jpg  "Readmission – initial days")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_ReAdmis-TotalCharge.jpg "Treatment-InitialDays")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_Treatment-Initial_days.jpg "Treatment-InitialDays")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/corr_matr.jpg "Heatmap")

## Summary
Discuss the results of the hypothesis test.
A contingency table was created of both "Services" (independent variable) and "ReAdmis" (dependent variable) factors.  The "chi2_contingency" hypothesis test was selected because of its ability to work with discrete variables. The resulting p-value is 0.031 and alpha is .05.  The Null hypothesis is rejected because the p-value is less than alpha, albeit by a small amount. This means there is a significant difference in the distribution between the “Services” factor for "ReAdmis" values.  The contingency table shows patients that received either a “CT Scan” or an “MRI” were more likely to be readmitted into the hospital later. 

##  Limitations
The p-value of 0.031 does meet the minimum threshold.  This suggests a possible relationship between the services received and readmissions rates which requires further investigation.  

## Recommendations
Further analysis is required to determine whether a true relationship exists. Hospital staff recommended to monitor patients that received CT or MRI scans in order to identify possible patterns. 

## Sources for third-party code:
1.	Tutorialspoint (p. 1). ML - Understanding Data with Visualization
https://www.tutorialspoint.com/machine_learning_with_python/machine_learning_with_python_understanding_data_with_visualization.htm
2.	Sani Kamal (2019, Multiple pages). Introduction to Multivariate Analysis
https://www.kaggle.com/sanikamal/introduction-to-multivariate-analysis

## Sources
1.	Saunders ND, Nichols SD, Antiporda MA, Johnson K, Walker K, Nilsson R, Graham L, Old M, Klisovic RB, Penza S, Schmidt CR. (October 15, 2011–April 15, 2012). Examination of Unplanned 30-Day Readmissions to a Comprehensive Cancer Hospital. https://ascopubs.org/doi/10.1200/JOP.2014.001546

2.	Mary MchHugh (Jun, 2013, Section: Introduction). The Chi-square test of independence
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3900058
