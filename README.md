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
Here are boxplots of some of the categorical features:

![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_ReAdmis-Initial_days.jpg  "Readmission – initial days")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_ReAdmis-TotalCharge.jpg "Treatment-InitialDays")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/boxplot_Treatment-Initial_days.jpg "Treatment-InitialDays")
![alt text](https://github.com/smithjs135/D207---Hospital-Readmissions-/blob/main/corr_matr.jpg "Heatmap")

