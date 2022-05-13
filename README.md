# databootcamp-school-district-analysis

## Project Overview
### Background
The school board of School District ISD would like to make sense of the academic data collected from the 9th - 12th grade students across all high schools within the district. They've provided the raw data and have reached out for assistance in parsing, analysing, and summarzing the key performance metrics. 

### Objective
The purpose of this project was to deliver easy-to-read performance metrics of high schools within the district. This report will serve as a benchmark of current performance as well as provide insight on the effects of budget, school size, school type, and budget on student scores. 

#### Challenge - Data Scrubbing
After a first pass of the data, the disctrict board members discovered a discrepancy in scores for Thomas High School ninth graders and flagged this as a possible indication of academic dishonesty. They requested, as a response, that the Thomas High School ninth grade scores be scrubbed from the original data. The final analysis uses scrubbed numbers as to get the most accurate analysis possible for district decision making. 

### Resources
Link to resources provided by client here: https://github.com/mcdoralds/databootcamp-school-district-analysis/tree/main/Resources

Python 3.7, Anaconda, Jupyter Notebook

## Results
As mentioned, the district board discovered potential academic dishonesty after the first pass of data reports and wanted to exclude a certain set of data from the analysis. They requested a re-run once the scores in question were removed from the overall DataFrame. The following changes were observed after the data was "scrubbed" :

- When 9th graders' math and reading scores were excluded, **the overall passing percentage for Thomas High School fell from 90.9% to 65.1%.** 



The delta in the two reports further support the board's hypothesis that there is abnormal activity in Thomas High School ninth graders' scores.



## Summary
