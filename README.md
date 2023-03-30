# pandas-challenge
## Andrew Lounsbury
Module 4 Pandas challenge for the Vanderbilt Data Analytics Bootcamp

# Code from Stack Overflow
The cell 
```
# Use `pd.cut` to categorize spending based on the bins.
# https://stackoverflow.com/questions/75808415/why-am-i-getting-typeerror-not-supported-between-instances-of-int-and-st
# We're trying to compare the integer bins to the budgets, which have dollar signs in them, making them strings. To avoid this, we take just the numbers in the string with .str[1:], and convert just that portion to a float. Then the comparison works. 
school_spending_df["Spending Ranges (Per Student)"] = pd.cut(school_spending_df["Per Student Budget"].str[1:].astype(float), bins=spending_bins, labels=labels)
school_spending_df
```
contains some code taken from [this page](https://stackoverflow.com/questions/75808415/why-am-i-getting-typeerror-not-supported-between-instances-of-int-and-st). 