<h2>Kaggle-GiveMeSomeCredit</h2>
<h3>Description:</h3>
A brief look at the Give Me Some Credit dataset from Kaggle. 
Incorrect data was imputed and outliers removed. Subsequently a 2-fold cross validation was applied and various models were fitted such as Logistic Regression, Random Forest, XGBoost. Further an Ensemble and Stacking was tried.


<h3 id="System Objective">Introduction</h3>
The 3 month long contest from Kaggle called <a href="https://www.kaggle.com/c/GiveMeSomeCredit/overview/description">Give Me Some Credit (GMSC)</a> involves predicting the probability that a person within 2 years did not repay an installment paying in 90 days or more beyond the due date. 
There are 11 bits of historical data with about 250,000 anonymous borrower information occupying 15MB and 5MB compressed hard drive space. The dataset is split into 150,000 examples (labeled training set - with 10,026 positive and 139,974 negative elements) and testing rows of 101,503. The following table summarises the numeric dataset with one predictor variable called <em>SeriousDlqin2yrs</em> and 10 explanatory variables (features).
        
<style type="text/css">
	table.tableizer-table {
		font-size: 12px;
		border: 1px solid #CCC; 
		font-family: Arial, Helvetica, sans-serif;
	} 
	.tableizer-table td {
		padding: 4px;
		margin: 3px;
		border: 1px solid #CCC;
	}
	.tableizer-table th {
		background-color: #104E8B; 
		color: #FFF;
		font-weight: bold;
	}
</style>
<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>Variable Name</th><th>Description</th><th>Data Type</th></tr></thead><tbody>
 <tr><td>SeriousDlqin2yrs</td><td>Person experienced 90 days past due delinquency or worse.</td><td>Y/N</td></tr>
 <tr><td>RevolvingUtilizationOfUnsecuredLines</td><td>Total balance on credit cards and personal lines of credit except real estate and no installment debt like car loans divided by the sum of credit limits.</td><td>percentage</td></tr>
 <tr><td>Age</td><td>Age of borrower in years.</td><td>integer</td></tr>
 <tr><td>NumberOfTime30-59DaysPastDueNotWorse</td><td>Number of times borrower has been 30-59 days past due but no worse in the last 2 years.</td><td>integer</td></tr>
 <tr><td>DebtRatio</td><td>Monthly debt payments, alimony,living costs divided by monthy gross income.</td><td>percentage</td></tr>
 <tr><td>MonthlyIncome</td><td>Monthly income.</td><td>real</td></tr>
 <tr><td>NumberOfOpenCreditLinesAndLoans</td><td>Number of Open loans (installment like car loan or mortgage) and Lines of credit (e.g. credit cards).</td><td>integer</td></tr>
 <tr><td>NumberOfTimes90DaysLate</td><td>Number of times borrower has been 90 days or more past due.</td><td>integer</td></tr>
 <tr><td>NumberRealEstateLoansOrLines</td><td>Number of mortgage and real estate loans including home equity lines of credit.</td><td>integer</td></tr>
 <tr><td>NumberOfTime60-89DaysPastDueNotWorse</td><td>Number of times borrower has been 60-89 days past due but no worse in the last 2 years.</td><td>integer</td></tr>
 <tr><td>NumberOfDependents</td><td>Number of dependents in family excluding themselves (spouse, children etc.).</td><td>integer</td></tr>
</tbody></table>

Since the class labels are provided for the sole response variable SeriousDlqin2yrs taking values 0 (NO default) or 1 (default). Supervised Learning classification models are a natural initial approach such as logistic regression as the base model and to improve with an ensemble of two-class boosted decision tree and stacking techniques involving Neural Networks.



<thead><tr class="tableizer-firstrow"><th></th></tr>
</tbody></table>



<h3>Requirements</h3>
 <p><a href="https://www.python.org/">Python (>3.4)</a>, <a href="https://jupyter.org/">jupyter</a> and <a href="https://scikit-learn.org/">SciKitLearn</a>.</p>
 
 
