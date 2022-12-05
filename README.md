# Prosper Loans Dataset Exploration and Analysis

Link to the report: [Prosper Loans Dataset Exploration and Analysis](https://adogb.github.io/prosper-loans/)
See exploration.html for the initial exploratory analysis.

## Dataset

The dataset includes 110,000+ listings of consumer loans provided by Prosper, with information on the borrower and loan details and status, among others. I was only interested in looking at closed loans, so my deataset was actually 43,000+ listings.


## Summary of Findings

I found that more than 11% of closed loans in the dataset are unpaid loans, i.e. they were charged off or defaulted. This also corresponds to the percentage in dollar amount. The loan amount distribution is right-skewed, and so are the borrower's APR, the debt-to-income ratio, the loan-to-income ratio and the monthly income distributions. I found some unusally high incomes in the dataset which were filtered off. Most people in the dataset were employed and first-time borrowers on Prosper.
Most loans had a Prosper rating of D.

Looking at bivariate exploration, I found an expected moderate to high correlation between the loan amount and the loan-to-income ratio. However I could also see that even with relatively small loan amounts, some people incur a debt of more than 100% of their annual income.

There is a moderate positive correlation between the debt-to-income ratio and the loan-to-income ratio. This suggests that the more debt-to-income a person has prior to applying for a loan, the more money (compared to their income) they are borrowing. This could be explained by the fact that people borrow to consolidate their debt.

Borrowers with higher incomes also seem to borrow more. It seems counter-intuitive but it would make sense that Prosper would be more inclined to accept a loan application for high amounts for people with a higher monthly income.

More than the monthly income alone or the loan amount alone, the debt-to-income and loan-to-income ratios are better predictors of whether a loan will be repaid or not, especially in combination with one another. The higher both ratios, the more incidence of unpaid loans.

I also looked into the Prosper rating: the lower the ratings, the more unpaid loans. But for all ratings, the debt-to-income ratio was again a clear differentiator between paid and unpaid loans.

## Key Insights for Presentation

For the presentation I focus on the influence of debt-to-income ratio, the loan-to-income ratio and the Prosper rating on the incidence of unpaid loans.

I start by showing the bar chart with the frequencies of paid and unpaid loans, to give an overview of the problem.

I then show the relationship between the debt to income ratio and the loan status and Prosper rating, with violin plots. I also show the relationship between Prosper rating and loan status.

I finish by presenting how the two ratios combined influence the loan status, with a scatterplot with colors, and that the debt-to-income influence is seen across all loans independently of the Prosper rating.