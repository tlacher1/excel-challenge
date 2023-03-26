# Kick Starter Challenge
## Background
Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since the late 2000s. From independent content creators to famous celebrities, more and more people are using crowdfunding to launch new products and generate buzz, but not every project has found success.

To receive funding, the project must meet or exceed an initial goal, so many organizations dedicate considerable resources looking through old projects in an attempt to discover “the trick” to finding success. For this week's Challenge, you will organize and analyze a database of 1,000 sample projects to uncover any hidden trends.

## Solution
Conditional formatting was applied to the "Outcome" and "Percent Funded" columns with different color, depending on whether the associated campaign was successful, failed, canceled, or is currently live. The "Percent Funded" column was created to uncover how much money a campaign made to reach its initial goal.

<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/main/Kickstarter%20-%20conditional%20image.png">
</p> 

A pivotal table was created to see the counts of how many campaigns were initially successful, failed, canceled, or currently live per category. Also a stacked column pivot chart was added to filter by country based on the table.


<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/41f654501744b836b2fe7af250c00ac584f5d588/Pivot%20table.png" />
<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/41f654501744b836b2fe7af250c00ac584f5d588/Graph%20of%20category%20stats.png" />
</p>

A pivot table and chart were also created to analyze how many campaigns were successful, failed, or canceled, or are currently live per sub-category. 
<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/338f1dc2441b7594826d854e8d17d272939c8a16/Pivot%20table%20by%20sub%20category.png" />
<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/338f1dc2441b7594826d854e8d17d272939c8a16/Graph%20of%20subcategory%20stats.png" />
</p>

Updated dates within the "deadline" and "launched_at" columns from Unix timestamps format to Excel's date format.  The new datecolumns were named "Date Created Conversion" and "Date Ended Conversion".

A pivot table and chart were created with the column of "state" and rows of "Date Created Conversion" by month.  The values were based on the count of "state" and then filtered based on "parent category" and "Years".  A pivot chart line graph was then used to visualize the outcomes.

<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/ca1ce0bbcdb0cf80e7a199ae3c91b9c2c646aff7/Pivot%20table%20by%20total%20outcome%20based%20on%20launch%20date.png" />
<p align="center">
<img src="https://github.com/tlacher1/excel-challenge/blob/ca1ce0bbcdb0cf80e7a199ae3c91b9c2c646aff7/Line%20graph%20based%20on%20total%20outcome.png" />
</p>

## Conclusions

1. Draw three conclusions from the crowdfunding campaigns:

*   Plays are the most crowdfunded subcategory overall.

*   Overall 56.5 % of crowdfunded campaigns were successful according to the dataset.

*   Campaigns that have a set goal between 1000 and 4999 have a greater success rate with the highest number of total projects.

2. Define some of the limitations of the dataset:

*  The majority of the data set entries are US based campaigns which have a tendency to skew the results towards US interests.

*  Some categories are informationally under represented in the table such as journalism which has a 100% success rate, but there are only 4 campaigns.

3. What are some other possible tables and/or graphs thatcould be created and what additional value would they provide?

*  Display a table or graph that shows crowdfunding campaigns exclusively based on country. This will provided backers information specific to their home country’s success rate per category.
