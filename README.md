# databootcamp-school-district-analysis

## Project Overview
### Background
The school board of School District ISD would like to make sense of the academic data collected from the 9th - 12th grade students across all high schools within the district. They've provided the raw data and have reached out for assistance in parsing, analysing, and summarzing the key performance metrics. 

### Objective
The purpose of this project was to deliver easy-to-read performance metrics of high schools within the district. This report will serve as a benchmark of current performance as well as provide insight on the effects of budget, school size, school type, and budget on student scores. 

#### Challenge - Data Scrubbing
After a first pass of the data, the district board members discovered a discrepancy in scores for Thomas High School ninth graders and flagged this as a possible indication of academic dishonesty. In order to uphold state-testing standards, the district requested that the Thomas High School ninth grade scores be scrubbed from the original data. The final analysis uses scrubbed numbers as to get the most accurate analysis possible for district decision making. 

### Resources
Link to resources provided by client here: https://github.com/mcdoralds/databootcamp-school-district-analysis/tree/main/Resources

Python 3.7, Pandas and Numpy library, Jupyter Notebook

## Results
The district board members were pleased with the insight that the analysis provided, as it allowed them to easily pinpoint potential anomalies. At the first pass of the data, the district supervisor concluded that the students_complete.csv file shows evidence that reading and math grades for Thomas High School ninth graders have been altered. She requested that reading and math scores from Thomas High School 9th graders be replaced with "NaN"s (a null value) on the record. 

The following analysis is with "scrubbed" data that excludes the 461 THS 9th grade scores, which accounted for 1.17% of the total student population.

### Analysis
The per-school summary displays the merged DataFrames in single table by school in alphabetic order. 

![image](https://user-images.githubusercontent.com/31219195/170850562-7d19ca4a-a41f-45bd-9ab6-4e14e13d27b0.png)

The top 5 performing school with the highest overall % passing were all charter schools.

![image](https://user-images.githubusercontent.com/31219195/170850596-dbfc6685-1c5f-42ae-aa93-31471dd309a3.png)

The bottom 5 performing schools with lowest overall % passing were all district schools. 

The district board may find it of critical importance to improve the mathematics program for these schools, as the average math scores were significantly lower than average reading scores and there seems to be a consistently high failure rate in all 5 of these bottom-performing schools. 

![image](https://user-images.githubusercontent.com/31219195/170850635-bb67bd7d-98c5-43c2-9bc0-cdfc0d8e06f8.png)

Interestingly, the spending ranges didn't seem to be the issue for these bottom-performing schools. 

![image](https://user-images.githubusercontent.com/31219195/170850790-0bdd77cb-2bda-4a44-9995-ae0f348b49c3.png)

In fact, the per-student budget was, on average, higher for district schools than charter schools. This may indicate the need for district school commitees to band together and rethink the budget allocation for district schools.

A deeper look suggests that the issue is not the budget, but perhaps a staffing issue. A look at average scores and passing rates by school size shows that larger schools have significantly lower performance and passing rates, particularly with math.

![image](https://user-images.githubusercontent.com/31219195/170850815-c5b2cd9a-cccc-406c-8663-e53ab8690119.png)

### Key Takeaways

1. There are significant differences in passing rates and scores between charter and district schools.
![image](https://user-images.githubusercontent.com/31219195/170850882-01b7bb6b-996e-4700-9a44-582c23a23015.png)

2. Larger schools seem to have significantly lower math scores and lower passing math percentages compared to medium and small schools.
   - This does not immediately appear to be an issue of school budget, as lower performing schools have a higher per-student budget on average.
   - The failure rate of the lowest performing schools seem to skew heavily towards the mathematic scores, which further highlights the possible need to reformation of the math department for district schools.

3. Average reading & math scores appear to be consistent across grades, which shows the importance of school's overall availability of resources, help, and learning plan rather than focusing analysis on a particular grade or sub-group.

![image](https://user-images.githubusercontent.com/31219195/170851095-a1a43b77-e564-43f9-b416-c34ca0adb984.png)
