# School District Analysis
## Table of Contents
- [Overview of the Analysis](#overview-of-the-analysis)
    - [Purpose](#purpose)
    - [About the Dataset](#about-the-dataset)
    - [Tools Used](#tools-used)
    - [Description](#description)
- [Results](#results)
    - [District Summary](#District-Summary)
    - [School Summary](#School-Summary)
    - [Thomas High School’s performance relative to the other schools](#Thomas-High-School’s-performance-relative-to-the-other-schools)
    - [Math and reading scores by grade](#Math-and-reading-scores-by-grade)
    - [Scores by school spending](#Scores-by-school-spending)
    - [Scores by school size](#Scores-by-school-size)
    - [Scores by school type](#Scores-by-school-type)
- [Summary](#summary)
- [Contact Information](#contact-information)

## Overview of the Analysis
### Purpose:
The analysis generates district summary as well as per school summary on the math, reading, and overall passing percentages in the schools. 

After the initial analysis (in [PyCitySchools.ipynb](https://github.com/SohaT7/School_District_Analysis/blob/main/PyCitySchools.ipynb)), it was discovered that some academic dishonesty had occurred where the grades for the ninth graders had been altered. In order to maintain state-testing standards, these data values were replaced with NaNs (‘Not a number’) and the analysis ([PyCitySchools_Challenge.ipynb](https://github.com/SohaT7/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)) repeated.

### About the Dataset:
The dataset comprises of two CSV files, containing data on 14 different schools and students. The data file on schools has 14 records (one for each school) containing the fields: School ID, School Name, Type, Size, and Budget. The data file on students has 39170 records, containing the fields: Student ID, Student Name, Gender, Grade, School Name, Reading Score, and Math Score.

 - [Schools Data](https://github.com/SohaT7/School_District_Analysis/blob/main/Resources/schools_complete.csv)
 - [Students Data](https://github.com/SohaT7/School_District_Analysis/blob/main/Resources/students_complete.csv)

### Tools Used:
 - Python
 - Jupyter Notebook

### Description:
The total number of students in the initial analysis was 39170, whereas that in the analysis after fixing the data was 38709. The latter value has been used in the calculations done in the second analysis. 
The school_data_df and student_data_df were merged into a new dataframe called the school_compelte_dataset_df, and the two analyses carried out thereafter. 
For the second analysis, the math and reading scores for the ninth graders in Thomas High School have been replaced with ‘NaN’ (which stands for ‘Not a number’). The image below shows the first 15 rows from the student_data_df, which contain 3 rows with ‘NaN’ values therein.

!["NaNs"](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/NaNs.png)

## Results
### District Summary:
The district summary dataframe values are slightly changed after the fixture. The average math score is 79.0 (78.9 previously), the average reading score remains the same at 81.9, % Passing Math is 75.0 (not 74.8), % Passing Reading is 85.8 (not 85.7), whereas the % Overall Passing is 65.2 (as opposed to the previous 64.9).
The initial district summary is shown below:

![Initial District Summary](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/initial_district_summary_df.png) 

The district summary after the data fixture is as follows:

![District Summary post-fixture](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/district_summary_df.png)

### School Summary:
The per_school_summary_df below shows that the scores for each school remain the same as before, except for Thomas High School. For Thomas High School, there is a drastic improvement in the % Passing Math (93.2 from 66.9), % Passing Reading (97.0 from 69.7), and % Passing Overall (90.6 from 65.1) scores after the data has been fixed. 
The initial school summary is shown below:

![Initial School Summary](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/initial_per_school_summary_df.png)

The school summary after the data fixture is as follows:

![School Summary post-fixture](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/per_school_summary_df.png)

### Thomas High School’s performance relative to the other schools:
The top 5 schools remain the same as before: Cabrera High School followed by Thomas High School, Griffin High School, Wilson High School, and Pena High School respectively. Even though the % Overall Passing score for the Thomas High School has changed slightly (90.63 as opposed to 90.95 previously) after the data fixture, the score is still lower than that of Cabrera High School and higher than that of Griffin High School, hence it retains its second placement in the top 5 schools.
The initial top 5 schools and their scores are shown below:

![Initial top 5 schools](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/initial_top5_schools.png)

The top 5 schools and their scores, post-fixture are as follows:

![Top 5 schools post-fixture](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/top5_schools.png)

The bottom 5 schools are the same in both analysis, and in the order of: Rodriguez High School is the lowest performing school followed by Figueroa High School, Huang High School, Hernandez High School, and Johnson High School. 

![Bottom 5 schools](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/bottom5_schools.png)

### Math and reading scores by grade:
The Math and Reading scores by grade remain the same for schools except for Thomas High School, where the grades for 9th grade only have been replaced with ‘nan’.
The scores from the initial analysis are shown below:

![Initial math scores by grade](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/initial_math_scores_by_grade.png)

![Initial reading scores by grade](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/initial_reading_scores_by_grade.png)

The scores post-fixture are as follows:

![Math scores by grade](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/math_scores_by_grade.png)

![Reading scores by grade](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/reading_scores_by_grade.png)

### Scores by school spending:
The spending bins created are $0-586, $586-630, $631-645, and $646-675. The scores per spending bin (or level) remain the same as those before the data fixture. 

![Spending scores](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/spending_summary_df.png)

### Scores by school size:
The size bins created are small (<1000), medium (1000-1999), and large (2000-5000). The scores based on size bins i.e. level of student population in schools, remains the same as before.

![Size scores](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/size_summary_df.png)

### Scores by school type:
The type bins are created based on types of schools, i.e. charter and district. The scores based on types of schools remain the same before and after the data fixture. 

![Type scores](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/type_summary_df.png)

## Summary
To summarize, replacing the scores for ninth grade at Thomas High School results in almost negligible differences in the scores generated for district summary. The average math score has increased by 0.1 to 79.0, % Passing Math by 0.2 to 75.0, % Passing Reading by 0.1 to 85.8 (not 85.7), whereas the average reading score remains unchanged at 81.9. The % Overall Passing has increased by 0.3 to 65.2.

In contrast, the school summary shows considerable changes, but only for Thomas High School: the % Passing Math has increased from 66.9 to 93.2, the % Passing Reading has increased from 69.7 to 97.0, and the % Passing Overall has increased from 65.1 to 90.6 from 65.1. 

## Contact Information
Email: st.sohatariq@gmail.com







