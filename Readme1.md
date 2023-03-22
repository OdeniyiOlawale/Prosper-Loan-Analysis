# Prosper Loan Data Exploration

## Dataset
The dataset consists of 113937 records of Proper loans generated between the year 2005 - 2014. The dataset consists of information regarding each loan's listing and closing date, interest rate, loan original amount, prosper rating, loan status and several other variables. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv).

## Summary of Findings

During exploration, I started by looking at the distribution of the loan original amounts and I found out that on a log transform, there are fewer lower number of loans on the lower end ( $1,000 - $4,000), but with spikes just before $5,000, $10,000 and $15,000. Looking into the interest rate, I realised that majority of the interest rate on loans are between 5% and 30%. I then looked into the laon status variable and I found out that ~50% of all the loans are still active, 30% had already completed their loans while 10% of the loans had been chargedoff. Also, I find it interesting that more half of the prosper loans were taken to by borrowers to consolidate their debts. 

Of the 51 US states represented, the top10 states with the highest loan listing represented 55% of the entire loans listed. After investigating the amount of loans listed in each quarter of each year, I discovered that Q1 of 2014 had received more loan than any other quarter of the previous years, with the exception of Q4 of 2013.

While investigating the relationship between the Loan original amount and Interest rate a negative relationship was observed where lower loan amounts carried higher interest rates. A step further into the relationship between loan outcome and interest rate revealed a linear form of relationship in which all chargedoff, defaulted and past due loans generally had high interest rates. Important to note also is the fact that for chargedoff loans, there is a higher number (by implication, proportion) of the borrowers who do not belong to a group. This may suggest that being in a group reduces the chances of a loan becoming chargedoff later in the future.

Investigating the relationship between Loan Original Amount, Borrower Rate and Monthly Income, I realised that majority of the loans given to people who earn less than $10000 monthly are on the lower end, and they are the ones who generally repay more (they get higher interest rates). This relationship may explain why there are more bad loans as interest rate increases.

## Key Insights for Presentation

For the presetation. I focused mainly on the number of loans across several categories, the interest rate and loan outcome. I started by introducing the loan amount on a log transform, the Interest rate variable using a histogram, and showed I used a countplot to show the distribution of the loan status variable. 

Next, I reported the pattern of loan listings across the years, which showed 2013 to have the highest loan listing ever. I plotted the count of loans by quarter of each year, and I observed that Q1 of 2014 already has a very high count of loan listings compared to the previous years. Afterwards, I used a scatterplot to show the relationship between loan amount and interest rate. A violinplot of loan outcome vs. Interest rate proved useful as it revealed a postive relationship that suggests that a loan is likely to turn out bad if the interest rate is on the high side. I moved on to show the effectiveness of the prosper ratings in predicting a loan's outcome using a barchart. I went on to also display the outcome of loans granted across the years. 

Finally, I presented the Loan amount across interest rate and monthly income using a scatterplot by placing the monthly income  to adequate









