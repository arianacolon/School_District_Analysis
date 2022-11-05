# PyCitySchools with Pandas Analysis
## Overview of School District Analysis
Maria, a chief data scientist for a city school district, has asked me to assist her in analyzing data on student funding and students' standardized test scores. With this analysis, I will showcase trends of schools' performances, which will help the school board and superintendent make decisions regarding school budget and priorities. I will analyze the dataset to discover the following deliverables:
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
* The school summary dataframe was initially delivered as the following: ![image](https://user-images.githubusercontent.com/107401667/200098107-83d5c2a1-c769-45f8-806f-3f1124bf4765.png) . After changing the Thomas High School ninth graders reading and math scores to NaN, the dataframe is now presented as ![image](https://user-images.githubusercontent.com/107401667/200129015-5d94a48c-8e66-457a-bdea-3578eea87ab2.png) . This change only changed the metrics of Thomas High School. The values of the following metrics decreased: Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing. The value of Average Reading Score increased and the following Thomas High School metrics were not affected: School Type, Total Students, Total School Budget, & Per Student Budget.
*  ![image](https://user-images.githubusercontent.com/107401667/200129303-c0515373-bc47-4429-bcb9-562f9e2ddde9.png) Even though replacing the ninth graders' math and reading scores decreased Thomas High School's % Overall Passing, the school's performance relative to the other schools did not change. Thomas High School still has the second highest % Overall Passing.
* The following explains how other dataframes were affected by replacing the ninth-grade scores:
     * Math and Reading Scores by Grade:
          * Math: ![image](https://user-images.githubusercontent.com/107401667/200135277-9ed77d29-b2b6-455e-a154-3635a81d9d02.png)
          * Reading: ![image](https://user-images.githubusercontent.com/107401667/200135229-ff8dd62e-3f8d-4747-ae1d-33f6225b4074.png)
          * For both of these dataframes, the only value that changed from the original values is Thomas High School's 9th grade. In both of these, it now displays nan.
     * Scores by School Spending
          * ![image](https://user-images.githubusercontent.com/107401667/200136980-a4ccfab6-db37-4b72-a7c8-958a13ec4657.png) 
          * This dataframe was not affected by replacing the ninth-grade scores.
     * Scores by School Size
          * ![image](https://user-images.githubusercontent.com/107401667/200137055-2189e7a4-a92e-4487-bbbd-d82501213c81.png)
          * This dataframe was not affected by replacing the ninth-grade scores.
     * Scores by School Type
          * ![image](https://user-images.githubusercontent.com/107401667/200137099-da74aeff-a124-486c-ad60-04361eca70e4.png)
          * This dataframe was not affected by replacing the ninth-grade scores.
## Summary
After replacing the reading and math scores for the ninth grade at Thomas High School with NaNs, a main change caused in the school district analysis is how the % Passings decreased in the district summary. % Passing Math decreased by 0.2, % Passing Reading decreased by 0.3, and % Overall Score decreased by 0.1. A second change in the analysis is Average Reading Score for Thomas High School increased by 0.5 in the school dataframe summary. A third change in the analysis is how the total student count for the calculations decreased. The original student count was 39,170 students and dropped to 38,709 students after removing the ninth grade students of Thomas High School. A fourth change of the analysis is the Average Math Score for Thomas High School decreased by 0.06.
