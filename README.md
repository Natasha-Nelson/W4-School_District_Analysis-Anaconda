# W4-School_District_Analysis-Anaconda

## Overview of the school district analysis
The purpose of this analysis was to explore key metrics in school performance data in math and reading. Throughout this analysis, we look at the overall district performance, the performance of 15 high schools and other frameworks. In our initial phases, we assume that the scores for 9th graders at Thomas High School show evidence of academic dishonesty and should be dropped from the data set. In this analysis, we look at how school performance in terms of passing reading and/or math (scores >=70) is impacted by removing the scores of Thomas High School students in 9th grade. In addition to looking at overall district and school performance, we also examine grade averages at each school, performace by school type and school size. 

## Results 
### Impact on District Summary
The impact to the overall district summary from removing the scores of 9th graders at Thomas High School (referred to as 9 THS scores moving forward) is negligible as show by the figures below. The reason for this is that the number of 9th graders at Thomas High Schools is just over 450 of the approximately 39K students sampled. As these students account for 0.01% of all students in the district, the impact of removing these datapoints is minimal. 

 **fig 1: Initial District Summary**
 
![initial_district_analysis](https://user-images.githubusercontent.com/81983110/118418003-9ebc2200-b684-11eb-98be-895f66b09904.png)

**fig 2: Updated District Summary without 9 THS scores**

![clean_district_analysis](https://user-images.githubusercontent.com/81983110/118418001-9e238b80-b684-11eb-9efe-1241f2dce93e.png)

### Impact on School summary
In the school specific summary, the results for the other 14 schools in the district remain the same as conducted in the initial analysis so we will focus on the results for Thomas High only in this overview. As shown below, the average reading, average math and passing percentages for Thomas High School change less than 1% for all five of the metrics observed. Similar to the District Summary, the impact is negligible. This comparison is conducted between the initial dataset and an updated student total for calculating percentages (ie total students at Thomas High - # of 9th graders).

**fig 3: Initial Thomas High School Summary**

![initial_thomashigh](https://user-images.githubusercontent.com/81983110/118418614-11c69800-b687-11eb-968f-103c00243090.png)

**fig 4: Updated Thomas High School Summary**

![clean_thomashigh](https://user-images.githubusercontent.com/81983110/118418613-11c69800-b687-11eb-8674-778786d0f786.png)

### Impact on Relative Performance 
In both the initial research and in the 9 THS scores removed analysis, Thomas High School ranked second when focusing on the percentage of students passing both math and reading, despite the ~0.3% drop. It is worth noting that the schools ranked 1-6 in this district for overall passing percentages differ for less than 2% with over 90% of student passsing both subjects. For Thomas High School to have ranked in the bottom 5 schools in the district, the passing percentage would have to drop to 52-54%.

**fig 5: Initial Relative Performance Summary**

![initial_relativeperformance](https://user-images.githubusercontent.com/81983110/118418980-a41b6b80-b688-11eb-98ec-8c9c8754435a.png)

**fig 6: Updated Relative Performanc Summary**

![clean_relativeperformance](https://user-images.githubusercontent.com/81983110/118419004-c319fd80-b688-11eb-97b5-3e89ca63b6c4.png)

### Further Impacts on School Performance
#### Math and reading scores by grade
This analysis examine the average scores of students at each grade level by school. The only impact of this update to this framework was that there are no longer average scores for 9th graders at Thomas School because these values have been dropped. (see outputs 41 and 43 in PyCitySchools-Challenge.ipynb). 

#### Scores by school spending
The budget at Thomas High School per student was $638.00, including 9th grade students, putting Thomas High in the second highest spending bucket ($630-45). As shown by the figures below, there is no impact on the performance of this second highest tier by removing the 9 THS scores.

fig 7: Initial School Performace by Spending

![initial_percapita](https://user-images.githubusercontent.com/81983110/118420293-82bc7e80-b68c-11eb-930f-5598f823b612.png)

fig 8: Updaged School Performance by Spending

![updated_schoolbudget](https://user-images.githubusercontent.com/81983110/118420295-82bc7e80-b68c-11eb-9b3f-fae2696aa3f2.png)

#### School Size
As shown PyCitySchools-Challenge.ipynb by ouput 53 and 90, there is no substantial impact on performance by school size when removing the 9 THS scores. 

#### Scores by school type
As shown PyCitySchools-Challenge.ipynb by ouput 45 and 92, there is no substantial impact on performance by school type when removing the 9 THS scores.

## Summary
Across the four major analyses performed in this project, we found no major impact when removing the scores of 9th graders at Thomas High School. At the district level, we can easily account for this as the number of scores removed is such a small percentage. Similarly, when examing school performance by spending, size and school type, the 9th graders at Thomas High make up a small portion of the students surveyed. Unfortunately, we can't draw conclusions from these analyses as to whether 9 THS scores represent academic dishonesty. However, it is useful to know that this analysis overall has sampled a large enough population that conclusions for top performing schools hold true even with potential inflation for <500 students. 

Intriguingly, the performance metrics for Thomas High School did not change substantially between the initial analysis and when looking at upperclassmen (10-12th graders) only. As the 9th graders at Thomas High represent 28% of the school, we would expect to see these metrics drop if the 9 THS scores were inflated. This could indicate that academic dishonesty in this class was not widespread and is worth further examination. 
