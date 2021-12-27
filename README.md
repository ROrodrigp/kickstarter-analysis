# Kickstarting with Excel

## Overview of Project

### Purpose
The main purpose for the first module of the Boot camp is to analyze the kickstarters campaigns in relation to their launch dates and their funding goals so we can help Louise finding a specific trend using the Kickstarter dataset.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In the first place it was necessary to create a pivot table using all the kickstarters data. The launch date is equal to the column called "Date Created Convertion" so this is going to be in the rows part of the table. Automatically excel make the rows dividing the dates in semesters along all the years that we have, however we do not need this because the analysis is just about the months along all the years, so we need to eliminate the ohter divisions. Then the columns of the tables are the outcomes labels successful, failed and canceled and the values are the count of the outcomes. Lastly we add parent category and year as filters and select to filter by theater. 
<p align="center">
<img src="https://github.com/ROrodrigp/kickstarter-analysis/blob/3a2214ad8bd098426292ee73395e50dbd1aad5db/Resources/Captura%20de%20Pantalla%202021-12-26%20a%20la(s)%2020.14.17.png" widht="750" height="350">    
</p>
Then we add a line graph. Here you can appreciate that the number of theater Kickstarters canceled is very low in every month. It's also very clear that between May, June and July is the highest rate of successful outcomes then it decreases until reaches its lowest point in December. With this evidence it's possible to say that the best time to start a theater kickstarter is between May and June. The failed campaigns remains constant among every month, therefore we cannot make any recommendation about this category. 
<p align="center">
<img src="https://github.com/ROrodrigp/kickstarter-analysis/blob/0e5917a03e839f80988b908a3515b45d4b7ef002/Resources/Theater_Outcomes_vs_Launch.png" width="850" height="350">  
</p>  

### Analysis of Outcomes Based on Goals  
Here we are interested in the goal of each kickstarter hence we make different categories accordingly to the goal using the countif function for successful, failed and canceled projects. Then we make percentage of each outcome using the total number of projects.  
<p align="center">
<img src="https://github.com/ROrodrigp/kickstarter-analysis/blob/bf993b9dcefa99aff31212b06f3b47b10d18fc21/Resources/Captura%20de%20Pantalla%202021-12-26%20a%20la(s)%2021.09.15.png" width="700" height="250">  
</p>    

Next we add a line graph. We could expect that percentage failed line is directly proportional to the goal and the percentage successful line is inversely proportional to the goal and this is partially true but in the ranges 35000 to 39999 and 40000 to 44999 the trend changes. In this range the percentage successful line is higher than the percentage failed line and this is an odd behavior however we also have a lack of data in this section so this may be a reason for the change in lines.  
Another important detail is that between 15000 to 19999 exists the same percentage of successful and failed campaigns. We can say that below this goal point is more probable for a campaign to be successful (asking for a small amount of money) and above this goal point is more difficult for a campaign  to be successful.  
<p align="center">
<img src="https://github.com/ROrodrigp/kickstarter-analysis/blob/a0e1f1dc0f1b3dd99191ae339ce68703e9f85821/Resources/Outcomes_vs_Goals.png" width="700" height="250">  
</p>    

### Challenges and Difficulties Encountered
- When you are making a pivot table using dates Excel automatically returns dates by trimester or semester and this could be a little confusing, nevertheless you just have to drop this field and leave just the ones you need.   

- You can be confused using the countifs function because it can receive multiple conditions unlike countif that just have one single condition. 
- When you are making the percentages it is necessary to use iferror function for the cases when you have something divided by zero. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?  
First, May-June-July are the best months for launching a kickstarter theater campaign.   Second, there is none apparently trend between launch date and failed campaigns, which could mean that the failure in a Kickstarter campaign is not related with the date is launched 
- What can you conclude about the Outcomes based on Goals?
As expected, while kickstarters ask for small amounts of money the successful percentage reaches up 80% and the percentage decreases while the amount of money increases because is more difficult to collect the money.   
- What are some limitations of this dataset?  
There is a lack of data in kickstarters with a high goal. In the lowest goals there are up to 534 projects but in highest goals we barely have 9 projects. It is necessary to collect more data in this category so we can find a real trend. 

- What are some other possible tables and/or graphs that we could create?  
We could make a table and a graph line showing how the amount of total projects changes over the differents goals. There are just few projects asking for more than 3000.  
Another possibility could be a table with the outcome values according with the different campaign's durations. 
