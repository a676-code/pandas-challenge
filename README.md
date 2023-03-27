# pandas-challenge
## Andrew Lounsbury
Module 4 Pandas challenge for the Vanderbilt Data Analytics Bootcamp

# Code from Stack Overflow
The cell 
```
# Use `pd.cut` to categorize spending based on the bins.
school_spending_df["Spending Ranges (Per Student)"] = pd.cut(school_spending_df["Per Student Budget"].str[1:].astype(float), bins=spending_bins, labels=labels)
school_spending_df
```
contains some code taken from [this page](https://stackoverflow.com/questions/75808415/why-am-i-getting-typeerror-not-supported-between-instances-of-int-and-st). 