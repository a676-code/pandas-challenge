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

# Charts
## The Initial Data Set
![initial_df](images/1_df.png)
## District Summary
![district summary](images/2_district_summary.png)
## School Summary
![school summary](images/3_school_summary.png)
## Highest Performing Schools
![highest performing schools](images/4_highest-performing_schools.png)
## Bottom Performing Schools
![bottom performing schools](images/5_bottom_performing_schools.png)
## Math Scores by Grade
![math scores by grade](images/6_math_scores_by_grade.png)
## Reading Scores by Grade
![reading scores by grade](images/7_reading_scores_by_grade.png)
## Scores by School Spending
![scores by school spending](images/8_scores_by_school_spending.png)
## Scores by School Size
![scores by school size](images/9_scores_by_school_size.png)
## Scores by School Type
![scores by school type](images/10_scores_by_school_type.png)

# Report
* Overall, Charter schools greatly outperformed District schoools with Charter schools having an overall passing percentage of 90.43% and District schools having an overall passing percentage of 53.67%. 
* The school with the lowest number of students, Holden High School, had a high percent passing math (92.51%), an even higher percent passing reading (96.25%), and a relativley high percent overall passing (89.23%) despite its low spending rate per student (<585). 
* The school with the highest number of students had a low overall passing percentage (54.64%) despite having a higher spending range per student ($585-630) than Holden High School. 