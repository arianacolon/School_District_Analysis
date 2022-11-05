# PyCitySchools with Pandas Analysis
## Overview of School District Analysis
Maria, a chief data scientist for a city school district, has asked me to assist her in analyzing data on student funding and students' standardized test scores. With this analysis, I will showcase trends of schools' performances, which will help the school board and superintendent make decisions regarding school budget and priorities. I will present the following deliverables:
  * Snapshot of District's Key Metrics
  * Overview of Key Metrics for each School
  * Tables for each of the Following Metrics
      * Top 5 Performing Schools, based on Overall Passing Rate
      * Bottom 5 Performing Schools, based on Overall Passing Rate
      * Average Math Score Received by Students in each Grade at each School 
      * Average Reading Score Received by Students in each Grade at each School 
      * School Performance based on Budget per Student
      * School Performance based on School Size
      * School Performance based on Type of School  
### Purpose
Maria has been notified how the reading and math scores for Thomas High School ninth graders have been altered, equating to academic dishonesty. The purpose of this analysis is to replace these specific scores to NaNs, repeat the deliverables listed above, and analyze how these changes affected the overall analysis. 
## Resources
* Data Sources: schools_complete.csv, students_complete.csv
* Software: Jupyter Notebook (PythonData)
## Results
* The district summary dataframe was initially delivered as the following:![image](https://user-images.githubusercontent.com/107401667/200098034-6445989a-5d96-4fc9-9811-6e592c747aa1.png) . After changing the Thomas High School ninth graders reading and math scores to NaN, the dataframe is now presented as ![image](https://user-images.githubusercontent.com/107401667/200064032-98c407f7-96c6-4d98-bb08-b6a96c8fe310.png). This change did not affect the values of Total Students, Total Students, Total Budget, & Average Reading Score. However, the following metrics all decreased by at least 0.1: Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing. 
* The school summary dataframe was initially delivered as the following: ![image](https://user-images.githubusercontent.com/107401667/200098107-83d5c2a1-c769-45f8-806f-3f1124bf4765.png) . After changing the Thomas High School ninth graders reading and math scores to NaN, the dataframe is now presented as ![image](https://user-images.githubusercontent.com/107401667/200098339-03c873cb-ad0b-4bef-940e-73261143d34b.png). This change only changed the metrics of Thomas High School. The values of the following metrics decreased: Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing. The value of Average Reading Score increased and the following Thomas High School metrics were not affected: School Type, Total Students, Total School Budget, & Per Student Budget.



How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type
## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
