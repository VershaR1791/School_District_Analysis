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

- ###  District Summary:
  Before getting into aggregating data to create a district level summary of school district, the math and reading score for 9th graders of *'Thomas High School'* was replaced with *'NaN*' using *'loc*' function on the student dataframe. The new total number of students was calculated to determine the percentage passing rate in math and reading as well as the overall passing percentage in the district. Below is the snapshot of the district summary final dataframe after the change. Except the total student count the changes in other parameters such as *'Total budget', 'Average Scores'*  and *'% Passing'* does not change significantly. 
  ![District summary2](https://user-images.githubusercontent.com/84694664/126910623-df925b02-abe6-4e10-99d2-c7bccd19186d.JPG)

- ###  School Summary:
  The school summary provides a tabulated synopsis of each of the school in the district by *'School Type', 'Total Students', 'Total Budget', 'Budget per Student', 'Average Math & Reading Score'* and *'% passing in each subject'*. Here is a snapshot of all schools.
  ![school summary2](https://user-images.githubusercontent.com/84694664/126912189-d9509e31-8540-48f1-958a-78a34f142fb8.JPG)

  The top 5 performing schools are:
  ![Top schools](https://user-images.githubusercontent.com/84694664/126912233-9ab73179-5f64-4aa2-835e-4a280d55fe60.JPG)

  The bottom 5 performing schools are:
  ![bottom schools](https://user-images.githubusercontent.com/84694664/126912258-91874a11-d299-45c5-97d2-5ab1e5331d6a.JPG)

- ### Impact of replacing the 9th graders’ math and reading scores on Thomas High School’s performance:
  Removing the 9th graders' math and reading scores moved *'Thomas High School's'* rank from Rank 8 to Rank 2. Below is the snapshot of *'Thomas High School'* before and after removing the 9th grader's scores respectively.
  ![ths1](https://user-images.githubusercontent.com/84694664/126912839-14ff0fa5-1c73-40c9-b076-4a2e023c5b75.jpg)
  
  ![ths2](https://user-images.githubusercontent.com/84694664/126912886-a37c3be2-49f2-4a62-9687-3bf4e1bc102f.jpg)
  
- ### Impact of replacing the 9th grade scores on:
  - ### Math and reading scores by grade
    The math and reading scores are replaced by *'NaN'* for the 9th grade and the rest of the scores for other grades are unaffected. The overall average score for math and reading does not have a significant change.
    ![math score by grade](https://user-images.githubusercontent.com/84694664/126912945-842af259-18c8-445d-9305-00616d0aa542.JPG) ![reading by grade](https://user-images.githubusercontent.com/84694664/126913164-398f828c-c095-421e-b44a-c5d928af8000.JPG)

  - ### Scores by school spending
    The school spending was broken down into 4 spending ranges per student of *'<$584' , '$585-$629', '$630-$644'* and *'$645-$657'*. The lower the spend per student better the overall passing percentage of the school.
    ![score by school spending](https://user-images.githubusercontent.com/84694664/126913035-fe2f2599-4129-44c8-b8f1-03f7143083b5.JPG)

  - ### Scores by school size
    The school size consisted of 3 sizes *Small'<1000', Medium'1000-2000'* *'Large'2000-5000'* based on number of students. The medium and school size have a better overall passing percentage than larger size schools. 
    ![score by school size](https://user-images.githubusercontent.com/84694664/126913044-ff28a1f8-6151-43b8-a2b4-22e1273aba7e.JPG)

  - ### Scores by school type
    The school type is based on whether the school is *'District'* or *'Charter'*. The overall passing percentage is greater for Charter Schools than District schools by almost 40%.
    ![score by school type](https://user-images.githubusercontent.com/84694664/126913047-b485a0f7-b93f-41aa-ae61-cefbf9509e85.JPG)

## Summary: 
The four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School were replaced were:
- The rank of Thomas High School jumped from 8th to 2nd in the overall list.
- 

