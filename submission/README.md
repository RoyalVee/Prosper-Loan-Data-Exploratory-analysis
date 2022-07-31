# Prosper Loan Data Exploratory Analysis
## by Victor Oguche


## Dataset

The Prosper Loan dataset is a collection of loan records. Using the Prosper Loan dataset, Exploratory and Explanatory analysis was be carried out with the aim of finding trends, patterns and insight from the loan dataset. The Dataset contain 113937 row entries and 81 Columns. 

38 columns out of the orignal 81 columns was be used for this exploratory analysis.


- Nominal data:
LoanStatus
EmploymentStatus
IsBorrowerHomeowner bool
IncomeVerifiable bool
BorrowerState
Occupation
IncomeVerifiable bool

- Ordinal data:
ProsperRating
ListingCategory
IncomeRange



- Quantitative data
Term : 			The length of the loan expressed in months.
BorrowerAPR : 		The Borrower's Annual Percentage Rate (APR) for the loan.
BorrowerRate : 		The Borrower's interest rate for this loan.

LenderYield :		The Lender yield on the loan. Lender yield is equal to the interest rate on the loan less the servicing fee.	

EstimatedEffectiveYield : Effective yield is equal to the borrower interest rate (i) minus the servicing fee rate, (ii) minus estimated uncollected interest on 
charge-offs, (iii) plus estimated collected late fees.  Applicable for loans originated after July 2009.

EstimatedLoss: Estimated loss is the estimated principal loss on charge-offs. Applicable for loans originated after July 2009.

EstimatedReturn : The estimated return assigned to the listing at the time it was created. Estimated return is the difference between the Estimated
Effective Yield and the Estimated Loss Rate. Applicable for loans originated after July 2009.

ProsperScore : A custom risk score built using historical Prosper data. The score ranges from 1-10, with 10 being the best, or lowest risk score.  
Applicable for loans originated after July 2009.

CurrentDelinquencies : Number of accounts delinquent at the time the credit profile was pulled.

AmountDelinquent : Dollars delinquent at the time the credit profile was pulled.

DelinquenciesLast7Years : Number of delinquencies in the past 7 years at the time the credit profile was pulled.

AvailableBankcardCredit : The total available credit via bank card at the time the credit profile was pulled.

DebtToIncomeRatio : The debt to income ratio of the borrower at the time the credit profile was pulled. This value is Null if the debt to income ratio is not 
available. This value is capped at 10.01 (any debt to income ratio larger than 1000% will be returned as 1001%).


StatedMonthlyIncome : The monthly income the borrower stated at the time the listing was created.

TotalProsperLoans : Number of Prosper loans the borrower at the time they created this listing. This value will be null if the borrower had no prior loans.

TotalProsperPaymentsBilled : Number of on time payments the borrower made on Prosper loans at the time they created this listing. This value will be null if the 
borrower had no prior loans.

OnTimeProsperPayments : Number of on time payments the borrower had made on Prosper loans at the time they created this listing. This value will be null if 
the borrower has no prior loans.

ProsperPaymentsLessThanOneMonthLate : Number of payments the borrower made on Prosper loans that were less than one month late at the time they created this listing. 
This value will be null if the borrower had no prior loans.


ProsperPaymentsOneMonthPlusLate : Number of payments the borrower made on Prosper loans that were greater than one month late at the time they created this 
listing. This value will be null if the borrower had no prior loans.

ProsperPrincipalBorrowed : Total principal borrowed on Prosper loans at the time the listing was created. 
loans.

ProsperPrincipalOutstanding : Principal outstanding on Prosper loans at the time the listing was created. This value will be null if the borrower had no prior loans.

LoanCurrentDaysDelinquent : The number of days delinquent.

LoanOriginalAmount : The origination amount of the loan.

MonthlyLoanPayment : The scheduled monthly loan payment

PercentFunded : Percent the listing was funded.

Recommendations : Number of recommendations the borrower had at the time the listing was created.

InvestmentFromFriendsCount : Number of friends that made an investment in the loan.

InvestmentFromFriendsAmount : Dollar amount of investments that were made by friends.

Investors : The number of investors that funded the loan.

## Summary of Findings

> All the employment status category had a positive correlation in respect to Monthly Loan payment and original loan amount. Full-time employees are like to recieve more loans compared to part-time employee. So one's employment status is a key drive in recieving a personal loan. In addition, Income Range above 100,000 dollars tend to have more higher loan amount which is expected because of their income range.

>A huge amount of loan were taken for Debt Consolidation with Home improvemt trailing behind. More borrowers come for loan with the purpose of using it for Debt Consolidation.

> Across all income range the propser rating tends to increase with lower Borrower's Annual Percentage Rate (APR) for the loan. This trend shows a great impact on the Prosper Loan rating based off the Borrower APR and Income range.


> It was surprising to see that there was no distint significant pattern difference if a borrower home status ownership affects loan amount and monthly loan payment and same for the borrower income verification status. One would have expected some difference on the monthly loan payment for the home ownership status.

## Key Insights for Presentation

- Loan Original Amount Distribution
- Distribution of Stated Monthly Income
- Listing category distribution to get insight into what borrowers recieve loan to do.
- Loan Original Amount and Monthly Loan Payment distribution in respect to Employment Status
- Borrower APR across Prosper rating and Income Range
- 