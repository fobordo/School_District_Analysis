# School District Analysis

## Overview of School District Analysis
The purpose of the School District Analysis was to aid a City School District in analyzing the correlation between [student standardized test results data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/students_complete.csv) and [school district data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/schools_complete.csv) to provide performance trends and patterns that will help to inform School Board discussions and strategic decisions at the district level. The goal of the School District Analysis was to generate and observe summaries for the entire school district, individual schools, high and low performing schools, average math and reading scores by grade, scores by school spending per student, scores by school size, and scores by school type. The programming language Python, in conjunction with the open-source library Pandas, was used to analyze the standardized test results.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?

Original District Summary DataFrame:
![district_summary_df_original](/README_Images/district_summary_df_original.png)

New District Summary DataFrame:
![district_summary_df_new](/README_Images/district_summary_df_new.png)

### How is the school summary affected?

Original School Summary DataFrame:
![per_school_summary_df_original](/README_Images/per_school_summary_df_original.png)

New School Summary DataFrame:
![per_school_summary_df_new](/README_Images/per_school_summary_df_new.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Original School Summary DataFrame Filtered on Thomas High School:
![per_school_summary_df_ths_original](/README_Images/per_school_summary_df_ths_original.png)

New School Summary DataFrame Filtered on Thomas High School:
![per_school_summary_df_ths_new](/README_Images/per_school_summary_df_ths_new.png)

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade

Original Math Scores by Grade DataFrame Filtered on Thomas High School:
![math_scores_by_grade_ths_original](/README_Images/math_scores_by_grade_ths_original.png)

New Math Scores by Grade DataFrame Filtered on Thomas High School:
![math_scores_by_grade_ths_new](/README_Images/math_scores_by_grade_ths_new.png)

Original Reading Scores by Grade DataFrame Filtered on Thomas High School:
![reading_scores_by_grade_ths_original](/README_Images/reading_scores_by_grade_ths_original.png)

New Reading Scores by Grade DataFrame Filtered on Thomas High School:
![reading_scores_by_grade_ths_new](/README_Images/reading_scores_by_grade_ths_new.png)

#### Scores by school spending

Original Spending Summary DataFrame:
![spending_summary_df_original](/README_Images/spending_summary_df_original.png)

New Spending Summary DataFrame:
![spending_summary_df_new](/README_Images/spending_summary_df_new.png)

#### Scores by school size

Original Size Summary DataFrame:
![size_summary_df_original](/README_Images/size_summary_df_original.png)

New Size Summary DataFrame:
![size_summary_df_new](/README_Images/size_summary_df_new.png)

#### Scores by school type

Original Type Summary DataFrame:
![type_summary_df_original](/README_Images/type_summary_df_original.png)

New Type Summary DataFrame:
![type_summary_df_new](/README_Images/type_summary_df_new.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
### Change 1: district_summary_df
### Change 2: per_school_summary_df
### Change 3: math_scores_by_grade
### Change 4: reading_scores_by_grade
