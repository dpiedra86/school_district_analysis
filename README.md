# school_district_analysis
4th Bootcamp Challenge

#Overv#iew 

The purpose of this project was to understand how Jupyter Notebook works. 
Jupyter is a flexible interface allows users to configure and arrange workflows in data science, scientific computing, computational journalism, and machine learning, as described in their website. Jupyter combined with Python and it's vast pool of libraries allow the user to perform deep analysis by manipulating data from a any given source without actually editing the input data from the original source. 

The request was to create a deep analysis to understand how well the schools taking a districtal test perfromed. For this test we had a couple of data sets and the tool we were asked to use was Python and mainly Pandas libraries. With this, we had the right tools to manipulate the data in both datasets to merge, group, add, substract and compare along other operations we dide to understand with tbales and summaries the results obtained. 

## Results

### How is the district summary affected?

![Disctrict_Summary](https://github.com/dpiedra86/school_district_analysis/blob/main/Images/practice_district_summary.png)
District Summary All Schools

![Disctrict_Summary](https://github.com/dpiedra86/school_district_analysis/blob/main/Images/challenge_district_summary.png)
District Summary excluding THS 9th graders

> **Conclusion**: 
Only the passing percentages were affected, and it happened ina minor scale. THS does not represent a large amount of data so it is only perceptible by using decimal figures.

### How is the school summary affected?
 
![School_Summary](https://github.com/dpiedra86/school_district_analysis/blob/main/Images/practice_school_summary.png)

School Summary All Schools

![School_Summary](https://github.com/dpiedra86/school_district_analysis/blob/main/Images/challenge_school_summary.png)

School Summary excluding THS 9th graders

> **Conclusion**: At a school level the percentages are greatly affected. This means 9th grade was raising the numbers with high math and reading grades. 
> We could deep dive into this data to get more information if needed. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

![School_Summary](https://github.com/dpiedra86/school_district_analysis/blob/main/Images/THS_failed.png)

Thomas High School excluding THS 9th graders

> **Conclusion**: Without the 9th graders THS fails to pass the minimum of 70% overall.


## How does replacing the ninth-grade scores affect the following:
### Math and reading scores by grade
> **Conclusion**: Both math and reading appear to have "NaN" for 9th grade, making them unable to compare with the rest of 9th graders. 

### Scores by school spending, Scores by school size, Scores by school type
> **Conclusion**: In the overall percentages it seems to make little difference in the percentages as they represent a very small part of the datset. 

## Changes Summary
- Using .loc helped us to get specific information from the data set. Until the challenge the most we did was to gruopby method.
- np.nan is very useful tool to change values in data set, later we can change the value with more advanced nan methods. 

is_NaN = student_data_df.isnull()
row_NaN = is_NaN.any(axis=1)
rows_with_NaN = student_data_df[row_NaN]
rows_with_NaN
- Using axis to ge to get Nan information. Although there are other mothods, this I found in the internet and liked the most. 
- Understanding how dtypes affect the operations we are trying to do. If oneself is trying to do some operations with diferewnt dtypes, one will get stuck until the information matches and the values are congruent. 
- This happened to me in the student substraction. 
