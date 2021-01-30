# Kickstarter-Analysis
Performing analysis on Kickstarter data to uncover trends

## Overview of Project
The following analysis will assist Louise in moving forward with her Kickstarter Campaign to fund a play in the United States.

### Purpose
Louise is curious about the launch dates and the funding goals of other plays. Through this analysis, Louise will acquire the information needed to move forward with her play. She will know what part of the year plays have higher success of launching, as well as how much money she should ask for in order to fund her project. The objective of this analysis is the visualize the data, making it easier and quicker to read. 


## Analysis and Challenges
This analysis is executed through Microsoft Excel. With the use of pivot tables and pivot charts, specific data is separated from the origianl worksheet and visualized to summarize the findings. Through this process the only difficulties are navigating through Excel without much prior experience. The most difficult part is the correct use of formulas/functions. It becomes especially tricky when the contents of a formula become larger and hold different columns. For example, when using the COUNTIFS() function, data from three different columns in the orignial worksheet are needed to figure out how many plays required specific quantities of money. This process not only becomes easier after repitition and familiarity with the function, but also after watching a tutorial video or two to help grasp a better understadning.     


### Analysis of Outcomes Based on Launch Day 
The first step in preparing an 'Outcomes Based on Launch Day' chart is converting data from the 'launched_at' column and placing it in a new column labeled 'Years'. The function =YEARS() was used to convert the data in column S 'Date Created Conversion'.  Once the data is listed in its new column a pivot table is formed in  a new sheet. The pivot table is then filtered based on the Parent Category, in this case 'theater', and the new 'Years' column. The legend/column section of the pivot table contains data from the 'outcomes' field, while the axis/rows sections holds data from the 'Data Created Conversion'. The values section is also based on the 'outcomes' field. Below is an image of the pivot table that is created for the 'Outcomes Based on Launch Day' sheet. A line chart is used to visualize the data from the pivot table. 


### Analysis of Outcomes Based on Goals
A new sheet is made  that will assist in the visualization of data for 'Outcomes Based on Goals'. The first column in the new sheet focuses on dollar-amount ranges in order to separate projects based on their goal amount. The following three columns are 'Number Successful', 'Number Failed' and 'Number Canceled'. These three columns represent the outcome of each project based on their financial goals. The fifth column is the total amount of projects per a specific financial range. The final three columns in the new 'Outcomes Based on Goals' sheet represent the percentage of projects that were successful, failed, or were canceled. The function =COUNTIFS() is used to convert data in the 'Kickstarter' sheet from three different columns. Those columns are 'outcome', 'goal' and 'Subcategory' (filtered to display 'plays'). The =SUM function is sused to count the total projects per financial range. A line chart is used to display the data with the financial range on the x-axis and percent on the y-axis. 


### Challenges and Difficulties Encountered
The most difficult part of this challenge is maintaining focus while using the =COUNTIFS function. This particular function is quiet large due to the fact that it holds three different criteria. Once the criteria are entered correctly, the function is not to challenging to repeat. 


## Results

### Outcomes Based on Launch Day
According to the data, Louise would give her project the best chance of being successful if she launches it during the months of May through July. Most successful plays are launched in this late spring/early summer period. May is the month with the most amount of successful plays, reaching 111 projects. June has 100 successful prjects and July has 87. It can be concluded that Louise would best benefit from launching project during the month of May. 

![image](Kickstarter/Theater_Outcomes_vs_Launch.png) 

### Outcomes Based on Goals
There are two financial ranges that would suggest higher success rates for plays in the 'Kickstarter' data. The first range includes plays that had lower financial goals. Plays that hope to fund their projects for less than $5,000 have around a 75% chance of being successful. The next highest range is for prijects that hope to fund their projects for $35,000 to $40,000. Their success rate was around 67%. From the data analysed, Louise would have a successful project with a funding goal of under $5,000. 

![image](Kickstarter/Outcomes_vs_Goals.png) 

### Limitations
There is more data available in the original 'Kickstarter' data set which could be used to draw more conclusions for Louise's project. Louise is hopeful that her play is successful in the United States, however she is also a big fan of British theater. There is sufficient data that is unused in this analysis which could give her an idea of the success rate in specifics locations. 

### Possibile Tables or Graphs 
For furthur analysis, a filter based on the location of projects could be incorporated into an analysis to determine how financial goals differ in specific countries. It has been suggested by the analysis that there are two ranges of less that $5,000 and in between $35,000 to $40,000 to funs a successful play. If there is a filter included to determine the location of these ranges, it maybe possible to conclude that a locaiton desires more or less funding to lead to a successful project. 
