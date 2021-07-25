# School_District_Analysis
Use Pandas to analyze school district data and provide recommendations

## Overview of the school district analysis
Maria is a Chief Data Scientist for the City School District. She has been tasked with the responsibility to analyze school district data which is available in different formats and from different sources. She is required to analyze standardized test data (for math & reading) as well as the school funding information, to report on performance trends and provide insights about patterns which will be used to inform decisions and strategies at school and/or district level by the school board. This analysis aggregates the data and help plan school budgets and priorities using Pandas and Jupyter Notebook. The analysis will include -
- **Data aggregation**  - import the data for school and students from excel and merge into one dataframe,
- **Data wrangling** -
  - clean the student data to remove preffixes and suffixes from names and,
  - remove 9th grad student's math and reading scores for *Thomas High School*, since they were incorrectly reported.
- **Data analysis** -
  - create a summary of student and school data,
  - identify high & low performing school through trends,
  - summarize school data by grade,
  - analyze school spend and provide a summary, and
  - analyze student scores by school size and school type.

## Results

- ###  District Summary
  Before getting into aggregating data to create a district level summary of school district, the math and reading score for 9th graders of *'Thomas High School'* was replaced with *'NaN*' using *'loc*' function on the student dataframe. The new total number of students was calculated to determine the percentage passing rate in math and reading as well as the overall passing percentage in the district. Below is the snapshot of the district summary final dataframe after the change. Except the total student count the changes in other parameters such as *'Total budget', 'Average Scores'*  and *'% Passing'* does not change significantly. 
![District summary2](https://user-images.githubusercontent.com/84694664/126910623-df925b02-abe6-4e10-99d2-c7bccd19186d.JPG)

- ###  School Summary
  The school summary provides a tabulated synopsis of each of the school in the district by *'School Type', 'Total Students', 'Total Budget', 'Budget per Student', 'Average Math & Reading Score'* and *'% passing in each subject'*. Here is a snapshot of all schools.
![school summary2](https://user-images.githubusercontent.com/84694664/126911360-b0641585-d31e-4578-8302-7eef248e014f.JPG)

- ### Impact of replacing the 9th graders’ math and reading scores on Thomas High School’s performance relative to the other schools

- ### Impact of replacing the 9th grade scores on:
  - ### Math and reading scores by grade
  - ### Scores by school spending
  - ### Scores by school size
  - ### Scores by school type

## Summary: 
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

