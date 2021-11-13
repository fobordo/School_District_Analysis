# School District Analysis

## Overview of School District Analysis
The purpose of the School District Analysis was to aid a City School District in analyzing the correlation between [student standardized test results data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/students_complete.csv) and [school district data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/schools_complete.csv) to provide performance trends and patterns that will help to inform School Board discussions and strategic decisions at the district level. The goal of the School District Analysis was to generate and observe summaries for the entire school district, individual schools, high and low performing schools, average math and reading scores by grade, scores by school spending per student, scores by school size, and scores by school type. The programming language Python, in conjunction with the open-source library Pandas, was used to analyze the standardized test results.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?

![district_summary_df_original](/README_Images/district_summary_df_original.png)
![district_summary_df_new](/README_Images/district_summary_df_new.png)

### How is the school summary affected?

![per_school_summary_df_original](/README_Images/per_school_summary_df_original.png)
![per_school_summary_df_new](/README_Images/per_school_summary_df_new.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
![per_school_summary_df_ths_original](/README_Images/per_school_summary_df_ths_original.png)
![per_school_summary_df_ths_new](/README_Images/per_school_summary_df_ths_new.png)

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
![math_scores_by_grade_ths_original](/README_Images/math_scores_by_grade_ths_original.png)
![math_scores_by_grade_ths_new](/README_Images/math_scores_by_grade_ths_new.png)

![reading_scores_by_grade_ths_original](/README_Images/reading_scores_by_grade_ths_original.png)
![reading_scores_by_grade_ths_new](/README_Images/reading_scores_by_grade_ths_new.png)

#### Scores by school spending
![spending_summary_df_original](/README_Images/spending_summary_df_original.png)
![spending_summary_df_new](/README_Images/spending_summary_df_new.png)

#### Scores by school size
![size_summary_df_original](/README_Images/size_summary_df_original.png)
![size_summary_df_new](/README_Images/size_summary_df_new.png)

#### Scores by school type
![type_summary_df_original](/README_Images/type_summary_df_original.png)
![type_summary_df_new](/README_Images/type_summary_df_new.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
### Change 1: district_summary_df
### Change 2: per_school_summary_df
### Change 3: math_scores_by_grade
### Change 4: reading_scores_by_grade
