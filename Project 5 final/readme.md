# Exploration of Loan Data from Propser
## by Olga Sawall


## Dataset

The loan data contains 81 columns, a significant amount of variables and characteristics that could be assosicated with each loan.

Most variables are numeric (float or int). But, there are also ordinal values like the ProsperRating (lowest - 0 - N/A, 1 - HR, 2 - E, 3 - D, 4 - C, 5 - B, 6 - A, 7 - AA - highest) or the ProsperScore (from 1-10, with 10 being the highest and 1 the lowest risk score).

There are also some numeric values that represent categorical data, e.g in the column ListingCategory (numeric): 0 - Not Available, 1 - Debt Consolidation, 2 - Home Improvement, 3 - Business, 4 - Personal Loan, 5 - Student Use, 6 - Auto, 7- Other, 8 - Baby&Adoption, 9 - Boat, 10 - Cosmetic Procedure, 11 - Engagement Ring, 12 - Green Loans, 13 - Household Expenses, 14 - Large Purchases, 15 - Medical/Dental, 16 - Motorcycle, 17 - RV, 18 - Taxes, 19 - Vacation, 20 - Wedding Loans.

The main feature for me was to analyse what is influencing the price (BorrowerRate) for the loan.


## Summary of Findings

The loan and interest rate distributions are slightly right skewed. Interestingly, some values stood out, like the interest rate of 32% oder the loan amounts of 4k, 10k and 15k USD. The distribution among rating categories is normal.

Monst of the loans were used for debt consolidation, but which acutally might be real estate loans as the percentage of homeowners among the borrowers increases over time (from 32% in 2007 to 50% in 2014). Additionally, the consolidation might take place to consolidate the high amount of credit lines (9-10 on average).

As expected, there is a clear relationship between interest and rating. Mean rate for the best category is approx. 7.5% and mean rate for the worst category is 32%. The mean rate only slightly increases with the term from 12% on 12 months to 18% on 60 months.

Also, loans with greater monthly installments have lower interest rates (as the rate increases, people want to repay faster). The price is also negatively correlated to the loan amount (i.e. greater loans show lower rates because they are mainly given to people with better rating categories).

The ranges for the means between the categories are significant with 15% beig the lowest for personal loans and 32% the highest for cosmetic procedures. The lowest mean loan amounts were given for student loans, bigger amounts were given (among others) for Baby&Adoption, Boats or Wedding Loans. Finaly, mean rates are slightly higher for defaulted and overdue loans.

Also, the interest varies greatly with the month, in which the loans was granted. In April, the mean interest rates were the lowest.

Reviewing further features I found that although the mean debt to income ratio decreases over time (from 36% in 2008 to 25% in 2014), and also mean monthly incomes increase over time (from 4500 USD in 2010 to 6000 USD in 2014) the mean interest rate actually does not decrease. Instead it slightly increases from 17% in 2006 to 20% in 2014.

I have plotted different variables to review what might influence the rating score. Debt to income ratio is strongly correlated with the rating, as well as the number of delinquencies. If the borrower was a homeowner, the rating was likely to be better. Also, if the borrower has not utilized the bankcard before. A full time employment is beneficial for a good rating (as "Part-Time" and "Retired" was only slightly better on the rating scala compared to "Not Employed"). And finally, the income also influences the rating category.

Over time, a significant increase was noticable especially for the good rating categories (7, 6, 5) with regard to debt ratio or stated income. For the lower rating categories (1, 2), actually debt ratio increased, as well as the percentage of homeowners (so I suppose many of them received real estate loans) - even though there was not a significant change in the monthly income over the years for these categories.

It seems that banks became more likely to provide loans to people: For borrowers with good rating the loan amounts increased over time, and this may be also covered by a positive financial development of the borrowers (monthly income, debt ratio). For borrowers with bad rating categories, loan amounts also increased over time. In these particular categories monthly incomes also increased over time, but so did the debt ratio and a greater percentage of borrowers became homeowners.


## Key Insights for Presentation

The presentation reviews the relationship between the loan amount, the interest rate and the rating. 

First, it shows the distribution of the loan amounts, the interest rates and the rating categories. 

In a second step it investigates the distribution of interest over rating categories. 

Additionally, it plots a scatterdiagram over loan amount and interest rate, using a color encoding over rating categories. 

It also plots the correlation between interest rate and term of the loan, as well as the loan repayment amount. Also it shows the change of interest rates over a year. 

In the next step, the presentation explores the relationship between rating and the features: delinquencies in the last 7 years, debt to income ratio, percentage of homeowners, bankcard utilization, employment status and monthly stated income.

Finally, the presentation shows the development of loan amounts and interest rates over year.