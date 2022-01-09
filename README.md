# Module 1: Kickstarter

Analyze a dataset consisting of 4,000 crowdfunding projects to discover hidden trends.

## Overview of project

The purpose of this project was to analyze data from the kickstarter_analysis.xlsx file to determine possible best fit for creating a successful kickstarter campaign for theater plays. The data I was interested in looking into was for two different relationships within the data. The first was the relationship between the month a kickstarter campaign began and the historical outcome for those projects. This could hopefully show when is the best time in the year to start a kickstarter campaign for plays. The second relationship of interest was the percentage of plays that succeeded, failed, or were canceled based on initial goal of the kickstarter campaign. This would help to understand what would be an appropriate goal ask for a play budget going into a kickstarter campaign.

## Analysis and Challenges

### Deliverable 1: Outcomes Based on Launch Date

#### Analysis

##### Data

The data was analyzed to determine outcomes based on start date by creating a pivot chart of worksheet 'kickstarter'. The pivot chart was created on a new worksheet called 'Theater Outcomes by Launch Date' The Filters for this chart were 'Parent Category' and 'Years. The Columns were set to 'outcomes' The Rows were set to 'Date Created Conversion' and the Values were set to 'Count of outcomes'. The data was also filtered to only depict the parent category value of 'theater'. The columns were filtered to remove 'live' theater kickstartes so that the only values that were left were 'successful', 'failed' and 'canceled'. The columns were also sorted into descending order based count of outcomes. The rows were organized from date created conversion into months.

##### Graph

The graph was created by using the data in the created pivot table. The graph was then copied and pasted into the microsoft paint application. The picture was then saved as 'Theater_Outcomes_vs_Launch.png. 

![Launch Date Pivot](https://github.com/drewabramo12/working_with_excel/blob/main/Theater_Outcomes_vs_Launch.png)

#### Challenge

The challenges that I ran into with creating this analysis were mostly adjusting to the novelty of new systems for myself. I had trouble with finding how to first change the row value to months. This was eventually found to be changed through group selection button on the top of the screen with the help of a hint within the instructions of the deliverable. I also had to go back through the work to determine why my data columns were not organized in the same way as the expected result. It took some fiddling with the filter prompt at the top of the column to figure that out. The last challenge of note for this deliverable was determining that the scaling of the graph for size needed to be done within the excel sheet. If the scale was changed in after converting to the paint application then the image became grainy.

### Deliverable 2: Outcomes Based on Goals Chart

#### Analysis

##### Data

The data was analyzed to determine outcomes based on goals by creating a new worksheet called 'Outcomes Based on Goals'. A chart was created with rows that depict groupings of values. These values start at 'Less than 1000' and then increase in intervals of 5000 until the cell 'Greater than 50000'. The Columns contain data that correlates for these values in the column information of 'Number Successful', 'Number Failed'. 'Number Canceled', 'Total Projects', 'Percentage Successful','Percentage Failed', and 'Percentage Canceled'.