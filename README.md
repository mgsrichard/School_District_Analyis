# School District Analyis

## Overview

Previously, we completed an analysis for a city school system of their students' outcomes in reading and in math. We computed average math and reading scores, and passing rates in math, reading, and overall passing in both subjects.  We presented these results on a city wide basis, individual school basis, by ranges of per capita spending, by school size, and by type of school (district vs. charter schools). Additionally, we provided a list of the top and bottom 5 performing schools. Now, they have contacted us again with concerns about the accuracy of the data from ninth graders at Thomas High School (THS), and asked us to do the analysis again excluding these student's grades. This report summarizes our findings with the scores from THS ninth graders omitted, and discusses the impact of that data change.

## Results

- How is the district summary affected?

The district summary is very slightly affected by the removal of the scores from 9th graders at THS.  The average reading score was unchanged, but the average math score, percentage of students passing math and reading, and the overall passing percentage all went down by very small amounts, between 0.1% and 0.3%. The following table summarizes the data elements that changed and how much they changed. You can also see the changes in the scores in the screenshots from the Jupyter Notebook output, which are attached below the table and labeled "Before" and "After."


|                   |Old Score  |New Score  |Change |
|-------------------|-----------|-----------|--------
|Average Math Score |79.0       |78.9      |0.1     |
|% Passing Math     |75.0       |74.8       |0.2    |
|%Passing Reading   |85.8       |85.7       |0.1    |
|%Passing Overall   |65.2       |64.9       |0.3    |

### Before
![Before district summary](https://github.com/mgsrichard/School_District_Analyis/blob/main/Before%20District%20Summary.png)
### After
![After district summary](https://github.com/mgsrichard/School_District_Analyis/blob/main/After%20District%20Analysis.png)

- How is the school summary affected?

In the school summary, only the THS scores are affected. The other schools' data is unchanged and so their scores are also unchanged.  A summary of the changes for THS is given in the following table, and you can also see the change in the screenshots of the school summaries before and after the THS 9th graders are removed.

|                   |Old Score  |New Score  |Change |
|-------------------|-----------|-----------|--------
|Average Reading Score|83.41     |83.35     |0.06   |
|Average Math Score |83.85       |83.90     |0.05     |
|% Passing Math     |93.27       |93.19       |0.06    |
|%Passing Reading   |97.31       |97.02       |0.29    |
|%Passing Overall   |90.95       |90.63       |0.32    |


### Before
![Before school summary](https://github.com/mgsrichard/School_District_Analyis/blob/main/Before%20School%20Summary.png)
### After
![After school summary](https://github.com/mgsrichard/School_District_Analyis/blob/main/After%20School%20Summary%20THS%20pcts%20right.png)

- How did replacing the ninth graders' math and reading scores affect THS's performance relative to other schools?

    Removing the ninth graders' math and reading scores did not change THS's rank as the second highest performing school, although it was very close.  Griffin High School, in 3rd place, is only 0.03% behind THS after the change and was 0.39% behind before.

### Before
![Before top 5](https://github.com/mgsrichard/School_District_Analyis/blob/main/Before%20Top%205%20schools.png)
### After
![After top 5](https://github.com/mgsrichard/School_District_Analyis/blob/main/After%20top%205%20schools.png)

- How does replacing the ninth-grade scores affect the following?
    - Math and Reading Scores by Grade
    
    The math and reading scores by grade are unaffected, except for the grades for the THS ninth graders, which are now replaced by NaNs (which means not a number).
    ### Before
    ![Before Math Scores](https://github.com/mgsrichard/School_District_Analyis/blob/main/Before%20Math%20scores%20by%20grade.png)
    ![Before reading scores bby grade](https://github.com/mgsrichard/School_District_Analyis/blob/main/Before%20reading%20scores%20by%20grade.png)
    ### After
    ![After Math Scores by Grade](https://github.com/mgsrichard/School_District_Analyis/blob/main/After%20Math%20Scores%20by%20school.png)
    ![After Reading scores by grade](https://github.com/mgsrichard/School_District_Analyis/blob/main/After%20Reading%20scores%20by%20school.png)
    - Scores by School Spending, School Size, and School Type
    
    The scores by school spending, school size, and school type are also unaffected by the removal of the these scores.  A total of 461 students' scores were removed, which represents only 1.1% of the entire school district population. For these calculations, however, the averages were computed with each school having an equal weight, which tended to lessen the weight of this large school in the outcome.  If weighted averages by school student counts were used instead, a very small change might be seen, but likely not a significant one.  
    
## Summary - Summarize 4 changes in the updated school district analysis after reading and math scores for ninth graders at THS have been replaced with nans

In summary, the removal of math and reading scores for the ninth graders at Thomas High School resulted in the following changes:
-  On a district level, the average math score, the passing percentage in math, the passing percentage in reading, and the overall passing percentage all declined slightly
-  For THS, the average reading score, average math score, the passing percentage in math, the passing percentage in reading, and the overall passing percentage all declined slightly
-  The student count is now 38,709 instead of 39,170, reflecting the removal of the 461 ninth graders from THS
-  THS's rank remained second among the schools in the district, but because the overall passing percent went down, their score is now very close to Griffin High School.
-  The average grades by school now reflect no scores for ninth graders at THS, showing nan (not a number) instead of the original scores
    
 A final thought: we didn't replace any data for THS, we only omitted it. Perhaps the real question, which we don't have the data to answer, is what would the scores have been if they were not altered or tampered with, and would that data have a greater impact on THS's performance and the school district as a whole?
    

