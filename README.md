# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this project was to analyze data from the kickstarter_analysis.xlsx file to determine possible best fit for creating a successful kickstarter campaign for theater plays. The data I was interested in looking into was for two different relationships within the data. The first was the relationship between the month a kickstarter campaign began and the historical outcome for those projects. This could hopefully show when is the best time in the year to start a kickstarter campaign for plays. The second relationship of interest was the percentage of plays that succeeded, failed, or were canceled based on initial goal of the kickstarter campaign. This would help to understand what would be an appropriate goal ask for a play budget going into a kickstarter campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

#### Data

The data was analyzed to determine outcomes based on start date by creating a pivot chart of worksheet 'kickstarter'. The pivot chart was created on a new worksheet called 'Theater Outcomes by Launch Date' The Filters for this chart were 'Parent Category' and 'Years. The Columns were set to 'outcomes' The Rows were set to 'Date Created Conversion' and the Values were set to 'Count of outcomes'. The data was also filtered to only depict the parent category value of 'theater'. The columns were filtered to remove 'live' theater kickstartes so that the only values that were left were 'successful', 'failed' and 'canceled'. The columns were also sorted into descending order based count of outcomes. The rows were organized from date created conversion into months.

#### Graph

The graph was created by using the data in the created pivot table. The graph was then copied and pasted into the microsoft paint application. The picture was then saved as 'Theater_Outcomes_vs_Launch.png. 

![Launch Date Pivot](https://github.com/drewabramo12/working_with_excel/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

#### Data

The data was analyzed to determine outcomes based on goals by creating a new worksheet called 'Outcomes Based on Goals'. A chart was created with rows that depict groupings of values. These values start at 'Less than 1000' and then increase in intervals of 5000 until the cell 'Greater than 50000'. The Columns contain data that correlates for these values in the column information of 'Number Successful', 'Number Failed'. 'Number Canceled', 'Total Projects', 'Percentage Successful','Percentage Failed', and 'Percentage Canceled'. The values of the cells took the formula `=COUNTIFS(Kickstarter!$F:$F, "successful",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<5000",Kickstarter!R:R,"plays")` in which three to four criteria and ranges are used to specify the number of outcomes within each specific criteria. Three criteria were used for rows contain 'less than 1000' and 'greater than 50000'. Four criteria was used in rows that are between two incremental boundaries. The first criteria and range specified the term 'succesful', 'failed', or 'canceled' to look at in worksheet 'Kickstarter' Column F. The second and/or the third criteria/range specified the goal limits between less than 1000 currency based increments, 5000 currency based increments, and greater than 50000 currency based increments in column D. As a note the third criteria is applied to The final criteria and range within this formula specifies the subcategory value 'plays' in worksheet 'Kickstarter' Column R. Column E of worksheet 'Outcomes Based on Goals' used the formula and variants of `=sum(B2:D2)` to determine the total number of kickstarter campaigns per goal increment. The final three rows were calculated by running a variation of the formula `=B2/E2` where the value successful, failed, or canceled variable was divided by the total to be given a percentage.

#### Graph

The graph was created by taking the values found in columns F through Column G into a line graph. The graph was then copied and pasted into the microsoft paint application. The picture was then saved as 'Outcomes_vs_goals.png'.

![Launch Date Pivot](https://github.com/drewabramo12/working_with_excel/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

#### Challenges of Outcomes Based on Launch Date

The challenges that I ran into with creating this analysis were mostly adjusting to the novelty of new systems for myself. I had trouble with finding how to first change the row value to months. This was eventually found to be changed through group selection button on the top of the screen with the help of a hint within the instructions of the deliverable. I also had to go back through the work to determine why my data columns were not organized in the same way as the expected result. It took some fiddling with the filter prompt at the top of the column to figure that out. The last challenge of note for this deliverable was determining that the scaling of the graph for size needed to be done within the excel sheet. If the scale was changed in after converting to the paint application then the image became grainy.

#### Challenges of Outcomes Based on Goals

The challenges I ran into with this creating this analysis was in determining the correct criteria for the countifs formulas. I went back and forth on whether the upper criteria range should be `,<5000 or ,<=4999`. Upon looking at the data I realized that either option was acceptable as there were no decimal numbers that were used. The other issue was finding the final criteria of the formula and its variants `=COUNTIFS(Kickstarter!$F:$F, "failed",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<5000",Kickstarter!$R:$R,"plays")`. The criteria that was missing was the subcategory 'plays' which took some deliberation to figure out.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The conclusions that could be determined were that the kickstarter campaigns were the historical best and worst times of the year for starting in May and October respectively. There is also of note the the conclusion that the graph follows a similar trend among all three lines. The upticks and downticks in the successful and failed lines at similar points that other kickstarter campaigns tend to follow a similar yearly pattern in start months. The three main times that theater kickstarter campaigns begin is in February, May, and October.

- What can you conclude about the Outcomes based on Goals?

The outcomes based on goals were that the best range to shoot for as your goal is somewhere in the range of 1000 to 4999 units of currency as multiple countries are express within this analysis.

- What are some limitations of this dataset?

Some limitations of note are that in the Outcomes based on Goals deliverable. As the monetary value goes up, there is a massive decrease in population which means that the percentages become less helpful in determining whether the goal is actually likely succeed or fail. Another limitation is that the data for plays in compared across all countries of this data set. It means that value of the currency is not accounted for in this analysis. It would also be worth mentioning that this across a 9 years of data. Inflation should be accounted for when evaluating earlier years versus more current years.

- What are some other possible tables and/or graphs that we could create?