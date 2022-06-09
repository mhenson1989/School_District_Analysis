# **School District Analysis**
## **Project Overview**

Within this project, I was tasked to perform an analysis of 15 different schools of various sizes and types and do a comparative analysis of average math and reading scores, looking specifically at passing rates, as well as school budgets. Additionally, this analysis factored in a consideration for the invalidity of the math and reading scores for the 9th grade class at Thomas High School. The purpose of this analysis was to create these summarys of information, while excluding this bad data from the data set. 

## **Results**
### *How is the district summary affected?*
Removing the 9th grade class from Thomas High School excluded 461 students from the overall student count of 39,170, making the new student count 38,709. This removal consequently effects the calculations for average math and reading scores, as well as the percentages of passing math, reading and overall passing, by changing the denominator of these equations. This would also effect the summation of the student count within the Total Students Column of the DataFrame. 

![Count Code Snippet](https://github.com/mhenson1989/School_District_Analysis/blob/main/Resources/NewStudentCount_codesnippet.PNG)

![Calculation Code Snippet](https://github.com/mhenson1989/School_District_Analysis/blob/main/Resources/NewStudentCount_PercentCalcs.PNG)

### *How is the school summary affected?*
Within the School Summary, the count and passing calculations for Thomas High School changed from a data set that included the addition of 461 9th grade math and reading scores, to an overall student count of 1,174, which only includes the 10th, 11th and 12th grade class. This adjusts Thomas High School's overall average math and reading scores, as well as their percent passing categories. This data change might be nominal in the aggrgate, however, it's important to note that it will more specifically effect data that looks at Per Student Spending Budgets, because it is eliminating an entire class where a spending budget per student is still applicable.

### *How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?*
Overall, replacing the math and reading scores for 9th graders at Thomas High School does not effect it's overall passing rating, in comparison to the initial analysis. Within the initial analysis, Thomas High School was rated as 2nd and within the new analysis, they are still rated as second. However, replacing these scores decreased their overall passing percentage from 90.948% to 90.630%. Though this percentage seems nominal, it creates a smaller gap between the number three school, Griffin High School, where their passing percentage is 90.599. 

![Top Five Code Snippet](https://github.com/mhenson1989/School_District_Analysis/blob/main/Resources/Top5.PNG)

### *How does replacing the ninth-grade scores affect the following:*
1. Math and reading scores by grade
    - In both the updated math and reading scores by grade dataframe, it reflects Thomas High School grades as NaN. 

2. Scores by school spending
    - Though Thomas High School will remain within the same spending budget bin, replacing the 9th grade scores will effect the calculations for average reading and math scores, as well as the passing percentages. However, the overall change in the averages and percentages are nominal, to the hundreths of decimal points and will be mostly rounded out in the final data set. 

![Spending Bins](https://github.com/mhenson1989/School_District_Analysis/blob/main/Resources/SpendingBins.PNG)

3. Scores by school size
    - Similarly to the school spending, Thomas High School remains within the same bin, however, it will marginally effect the average math and reading scores, as well as the percent passing rates. However, within the orginal analysis the rates are rounded to the whole number in the percent value and the tenth of a decimal point for average math and reading scores. So, when performing, similar rounding, there is no overall change within the aggregate. 

![School Size](https://github.com/mhenson1989/School_District_Analysis/blob/main/Resources/SchoolSize.PNG)

4. Scores by school type
    - There is no significant change to the scores by school type, looking to the thousandth decimal point. 

## Summary
Overall, removing the 9th grade data set from Thomas High School did not largely effect the aggregated data averages or percentages. Within the breakdown, you see the most significant (though not very significant) changes when reviewing overall student counts, overall passing percentages by school, specifically the gap between Thomas High School's current standing at second school and the third rated school, Griffin High School. Additionally, you see nominal change when reviewing the math and reading scores by school, by grade, and scores by school spending. 