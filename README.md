# School District Analysis

## Overview of the school district analysis
### Purpose of the analysis:
The analysis generates district summary as well as per school summary on the math, reading, and overall passing percentages in the schools. 
After the analysis, however, it was discovered that some academic dishonesty had occurred where the grades for the ninth graders had been altered. In order to maintain state-testing standards, these data values were replaced with NaNs (‘Not a number’) and the analysis repeated.
### Description of the analysis:
The total number of students in the initial analysis was 39170, whereas that in the analysis after fixing the data was 38709. The latter value has been used in the calculations done in the second analysis. 
The school_data_df and student_data_df were merged into a new dataframe called the school_compelte_dataset_df, and the two analyses carried out thereafter. 
For the second analysis, the math and reading scores for the ninth graders in Thomas High School have been replaced with ‘NaN’ (which stands for ‘Not a number’). The image below shows the first 15 rows from the student_data_df, which contain 3 rows with ‘NaN’ values therein.
!["NaNs"](https://github.com/SohaT7/School_District_Analysis/blob/main/Images/NaNs.png)



## Results:

## Summary:




For the second analysis, the math and reading scores for the ninth graders in Thomas HIgh School have been replaced with ‘NaN’ (which stands for ‘Not a number’). The image below shows the first 15 rows from the student_data_df, which contain 3 rows with ‘NaN’ values therein.
ADD IMAGE.


District Summary:
The district summary dataframe values are slightly changed after the fixture. The average math score is 79.0 (78.9 previously), the average reading score remains the same at 81.9, % Passing Math is 75.0 (not 74.8), % Passing Reading is 85.8 (not 85.7), whereas the % Overall Passing is 65.2 (as opposed to the previous 64.9).
ADD BOTH IMAGE.


Thomas High School’s Relative Performance:
The top 5 schools remain the same as before: Cabrera High School followed by Thomas High School, Griffin High School, Wilson High School, and Pena High School respectively. Even though the % Overall Passing score for the Thomas High School has changed slightly (90.63 as opposed to 90.95 previously) after the data fixture, the score is still lower than that of Cabrera High School and higher than that of Griffin High School, hence it retains its second placement in the top 5 schools.
ADD BOTH IMAGES.
The bottom 5 schools are the same in both analysis, and in the order of: Rodriguez High School is the lowest performing school followed by Figueroa High School, Huang High School, Hernandez High School, and Johnson High School. 


School Summary:
The per_school_summary_df below shows that the scores for each school remain the same as before, except for Thomas High School. For Thomas HIgh School, there is a drastic improvement in the % Passing Math (93.2 from 66.9), % Passing Reading (97.0 from 69.7), and % Passing Overall (90.6 from 65.1) scores after the data has been fixed. 
ADD BOTH 


The Math and Reading scores by grade remain the same for schools except for Thomas High School, where the grades for 9th grade only have been replaced with ‘nan’.
ADD IMAGES for THS only, and only if you want to.


The spending bins created are $0-586, $586-630, $631-645, and $646-675. The scores per spending bin (or level) remain the same as those before the data fixture. 
ADD Either ONE

The size bins created are small (<1000), medium (1000-1999), and large (2000-5000). The scores based on size bins i.e. level of student population in schools, remains the same as before as well.
ADD ONE.

The type bins are created based on types of schools, i.e. charter and district. The scores based on types of schools remain the same before and after the data fixture. 
ADD ONE.
