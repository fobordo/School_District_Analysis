# School District Analysis

## Overview of School District Analysis
The purpose of the School District Analysis was to aid a City School District in analyzing the correlation between [student standardized test results data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/students_complete.csv) and [school district data](https://github.com/fobordo/School_District_Analysis/blob/219964e5017a6b436c84949b13cd9051c158bb38/Resources/schools_complete.csv) to provide performance trends and patterns that will help to inform School Board discussions and strategic decisions at the district level. The goal of the School District Analysis was to generate and observe summaries for the entire school district, individual schools, high and low performing schools, average math and reading scores by grade, scores by school spending per student, scores by school size, and scores by school type. The programming language Python, in conjunction with the open-source library Pandas, were used to analyze the standardized test results.

After the initial analysis, it was discovered that the standardized test results for Thomas High School (THS) ninth-graders may have been altered. To uphold state-testing standards, all math and reading test scores for Thomas High School ninth-graders were replaced with NaNs, and the School District Analysis was repeated.

## Results:

### How the district summary was affected

The following district summary metrics did not change after repeating the analysis:
 * Total Schools
 * Total Students
 * Total Budget
 * Average Reading Score

However, the following district summary metrics were affected and changed slightly:
 * Average Math Score
 * % Passing Math
 * % Passing Reading
 * % Overall Passing

<p align="center">
 Original District Summary DataFrame
 <img src="/README_Images/district_summary_df_original.png">
</p>

The Original District Summary showed the following metrics:
  * Average Math Score: 79.0
  * Average Reading Score: 81.9
  * % Passing Math: 75.0%
  * % Passing Reading: 85.8%
  * % Overall Passing: 65.2%

<p align="center">
 Updated District Summary DataFrame
 <img src="/README_Images/district_summary_df_new.png">
</p>

The Updated District Summary showed the following metrics:
  * Average Math Score: 78.9
  * Average Reading Score: 81.9
  * % Passing Math: 74.8%
  * % Passing Reading: 85.7%
  * % Overall Passing: 64.9%

As seen in the above results for Original District Summary vs. Updated District Summary:
 * The Average Math Score decreased by 0.1.
 * The Average Reading Score did not change (if it did, it was by less than 0.05).
 * The % Passing Math decreased by 0.2%.
 * The % Passing Reading decreased by 0.1%.
 * The % Overall Passing decreased by 0.3%.

These changes were a reflection of the changes in metrics for Thomas High School, which we will analyze in the following sections.

### How the school summary was affected

The school summary metrics for Thomas High School were affected by the repeated analysis, but the metrics for all of the other schools stayed the same.

<p align="center">
 Original School Summary DataFrame
 <img src="/README_Images/per_school_summary_df_original.png">
</p>

<p align="center">
 Updated School Summary DataFrame
 <img src="/README_Images/per_school_summary_df_new.png">
</p>

As seen in the Original School Summary vs. Updated School Summary DataFrames above, the Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, and % Overall Passing metrics for Thomas High School changed after repeating the analysis, which we will analyze further in the next section.

### How replacing the ninth graders’ math and reading scores affected Thomas High School’s performance relative to the other schools

Replacing the ninth graders' math and reading scores affected Thomas High School's performance relative to other schools because the following THS metrics had to be recalculated:
 * Total number of THS students metric used in calculating Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, and % Overall Passing (ninth-graders were not counted)
 * Average Math Score
 * Average Reading Score
 * % Passing Math
 * % Passing Reading
 * % Overall Passing

<p align="center">
 Original School Summary DataFrame Filtered on Thomas High School
 <img src="/README_Images/per_school_summary_df_ths_original.png">
</p>

The Original School Summary showed the following metrics for THS:
  * Average Math Score: 83.418349
  * Average Reading Score: 83.848930
  * % Passing Math: 93.272171
  * % Passing Reading: 97.308869
  * % Overall Passing: 90.948012

<p align="center">
 Updated School Summary DataFrame Filtered on Thomas High School
 <img src="/README_Images/per_school_summary_df_ths_new.png">
</p>

The Updated School Summary showed the following metrics for THS:
  * Average Math Score: 83.350937
  * Average Reading Score: 83.896082
  * % Passing Math: 93.185690
  * % Passing Reading: 97.018739
  * % Overall Passing: 90.630324

As seen in the above results for Original School Summary vs. Updated School Summary for THS:
 * The Average Math Score decreased by 0.067412.
 * The Average Reading Score increased by 0.047152.
 * The % Passing Math decreased by 0.086481.
 * The % Passing Reading decreased by 0.29013.
 * The % Overall Passing decreased by 0.317688.

### How replacing the ninth-grade scores affected the following:
#### Math and reading scores by grade
The math and reading scores by grade for Thomas High School were the only metrics affected by repeating the analysis; the metrics for all other schools stayed the same.

<p align="center">
 Original Math Scores by Grade DataFrame Filtered on Thomas High School
 <img src="/README_Images/math_scores_by_grade_ths_original.png">
</p>

<p align="center">
 Updated Math Scores by Grade DataFrame Filtered on Thomas High School
 <img src="/README_Images/math_scores_by_grade_ths_new.png">
</p>

As seen in the Original Math Scores by Grade vs. Updated Math Scores by Grade DataFrames filtered on Thomas High School above, the grades for 9th grade previously showed 83.6, but now show "nan" after they were replaced with NaNs.

<p align="center">
 Original Reading Scores by Grade DataFrame Filtered on Thomas High School
 <img src="/README_Images/reading_scores_by_grade_ths_original.png">
</p>
 
<p align="center">
 Updated Reading Scores by Grade DataFrame Filtered on Thomas High School
 <img src="/README_Images/reading_scores_by_grade_ths_new.png">
</p>

Similarly, as seen in the Original Reading Scores by Grade vs. Updated Reading Scores by Grade DataFrames filtered on Thomas High School, the grades for 9th grade previously showed 83.7, but now show "nan" after they were replaced with NaNs.

#### Scores by school spending

The scores by school spending were not affected by replacing math and reading test scores for Thomas High School ninth-graders with NaNs and repeating the analysis, as seen in the Original Spending Summary vs. Updated Spending Summary DataFrames below.
 
<p align="center">
 Original Spending Summary DataFrame
 <img src="/README_Images/spending_summary_df_original.png">
</p>

<p align="center">
 Updated Spending Summary DataFrame
 <img src="/README_Images/spending_summary_df_new.png">
</p>

#### Scores by school size

The scores by school size were not affected by replacing math and reading test scores for Thomas High School ninth-graders with NaNs and repeating the analysis, as seen in the Original Size Summary vs. Updated Size Summary DataFrames below.

<p align="center">
 Original Size Summary DataFrame
 <img src="/README_Images/size_summary_df_original.png">
</p>

<p align="center">
 Updated Size Summary DataFrame
 <img src="/README_Images/size_summary_df_new.png">
</p>

#### Scores by school type

The scores by school type were not affected by replacing math and reading test scores for Thomas High School ninth-graders with NaNs and repeating the analysis, as seen in the Original Type Summary vs. Updated Type Summary DataFrames below.

<p align="center">
 Original Type Summary DataFrame:
 <img src="/README_Images/type_summary_df_original.png">
</p>
 
<p align="center">
 Updated Type Summary DataFrame
 <img src="/README_Images/type_summary_df_new.png">
</p>

## Summary:
In summary, the following four changes occurred in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School were replaced with NaNs.

### 1. District Summary
In the updated District Summary DataFrame, the metrics for Average Math Score, % Passing Math, % Passing Reading, % Overall Passing decreased by 0.1, 0.2%, 0.1%, and 0.3%, respectively.

### 2. School Summary
In the updated Per School Summary DataFrame, the Thomas High School metrics for Average Reading Score increased by approximately 0.05, while Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing decreased by approximately 0.07, 0.09%, 0.29%, and 0.32%, respectively.

### 3. Math Scores by Grade
In the updated Math Scores by Grade DataFrame, the math score for Thomas High School 9th grade was changed to "nan."

### 4. Reading Scores by Grade
In the updated Reading Scores by Grade DataFrame, the reading score for Thomas High School 9th grade was changed to "nan."
