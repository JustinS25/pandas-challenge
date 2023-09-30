# pandas-challenge

## Written Analysis

    When analyzing this data, we can gather a lot of information about the students and the schools within
this high school district. Loading in the csv files, I was able to use pandas dataframes to create detailed tables that includes information about everything from average math/reading scores by school, to total budget across all schools. To be more specific, we can outline how I created the several tables used in this assignment.
    To start, the starter code read in the files and provided us with a merged data frame using the 2
csv files we had. They were merged together using the "school_name" column. We then had to calculate several values to create a unique data frame with our created values. To calculate these values, we had to use several functions like .mean(), .unique(), and .count() to help us find the averages and amount of desired values.
    After creating the first data table, we were able to create one with a per school summary. Similarly
to the previous table, we had to use functions such as .mean() and .groupby() to group this data by school name.
    Afterwards, we wanted to create 2 seperate tables, sorted by ascending and descending overall passing 
percentages. This allows us to see which schools were best performing overall, and which were worst overall.
    We then created 2 data frames to see the mean scores by grade. This allowed us to see which grades at 
each school performed the best. To do this, we had to create merged data frames that incuded data grouped by school name. In order to get the specific grade, we had to ensure that we set a variable equal to the grade number prior.
    Next, we wanted to create a data frame to analyze the average scores in relation to per student 
spending. To do so, we had to create bins and use .cut() to see where each school would fall into. We then created a data frame that groups the data by spending range. By taking the tanspose and displaying the data, we were able to see the spending range per student and the corresponding average scores.
    For the last 2 data frames, we had to sort schools by school size and type. Similarly to the previous 
part, we had to sort by bins and use .cut() to place schools in bins by school size. We then created a data frame that groups data by school size and type, respectively, for the last 2 data frames, and sorted the average scores by size/types.

## Conclusions

    We can make several observations based off the resulting data. To start, we can look at the last data 
frame, which shows the average scores by school type. Because the data is so extreme, we can clearly see there is a better chance of passing math and reading by going to a charter school versus going to a district school. As a result, the better educational option seems to be going to a charter school.
    Another observation we can make is that the school size matters as well. Looking at the school size 
data frame, we can see that going to a large school often results in lower average scores than going to a small/medium sized school. Although we can't assume the exact cause, we can predict that going to smaller schools allows for a school to place more attention on each student as the student to teacher ratio is likely lower. We can also see from the data frames above that every district school is a large school and they all have low test averages. Could the causation of this low average be due to the school size, or is it likely due to the fact that many of the larger schools are district schools? There is still further reserach that can be done to get more definitive answers from this data, but as of now, we can make certain conlusions about school size/type in relation to student's test scores.


## Citations

- Used source code/variable names provided by professor as a guideline. Added various comments throughout.

- Looked up [transpose()](https://www.geeksforgeeks.org/python-pandas-dataframe-transpose/) function to use in data frames where I wanted to flip x and y axes:
https://www.geeksforgeeks.org/python-pandas-dataframe-transpose/

- Looked up [astype()](https://www.geeksforgeeks.org/python-pandas-dataframe-astype/) function to change data type of certain info within a data frame.:
https://www.geeksforgeeks.org/python-pandas-dataframe-astype/

- Rest of changes/info used was provided in source code/applied from class slides 4.1, 4.2, and 4.3
