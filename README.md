# Crowdfunding with Excel

Background

Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since the late 2000s. From independent content creators to famous celebrities, more and more people are using crowdfunding to launch new products and generate buzz, but not every project has found success.
To receive funding, the project must meet or exceed an initial goal, so many organizations dedicate considerable resources looking through old projects in an attempt to discover “the trick” to finding success. Analyze a database of 1,000 sample projects to uncover any hidden trends.

*Use conditional formatting to fill each cell in the outcome column with a different color, depending on whether the associated campaign was successful, failed, canceled, or is currently live.
**Create a new column called Percent Funded that uses a formula to find how much money a campaign made relative   to its initial funding goal.
  
*Use conditional formatting to fill each cell in the Percent Funded column according to a three-color scale. The scale should start at 0 with a dark shade of red, and it should transition to green at 100 and blue at 200.
**Create a new column called Average Donation that uses a formula to find how much each project backer paid on average.
**Create two new columns, one called Parent Category and another called Sub-Category, that use formulas to split the Category and Sub-Category column into the two new, separate columns.

<img width="1047" alt="image" src="https://github.com/MDCummings86/Crowdfunding/assets/126340452/d0f07874-90f4-451c-be4e-dd145f265fbb">


**Create a new sheet with a pivot table that analyzes your initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per category.

*Create a stacked-column pivot chart that can be filtered by country based on the table that you created.
Subcategory Stats

*Create a new sheet with a pivot table that analyzes your initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per sub-category.
*Create a stacked-column pivot chart that can be filtered by country and parent category based on the table that you created.
*The dates in the deadline and launched_at columns use Unix timestamps. Fortunately for us, this formula Links to an external site. that can be used to convert these timestamps to a normal date.
**Create a new column named Date Created Conversion that will use this formula Links to an external site. to convert the data contained in launched_at into Excel's date format.
**Create a new column named Date Ended Conversion that will use this formula Links to an external site. to convert the data contained in deadline into Excel's date format.

<img width="1044" alt="image" src="https://github.com/MDCummings86/Crowdfunding/assets/126340452/3e6f6c85-e665-49be-8611-ba05ea3cfc0f">


**Create a new sheet with a pivot table that has a column of outcome, rows of Date Created Conversion, values based on the count of outcome, and filters based on parent category and Years.
**Now, create a pivot-chart line graph that visualizes this new table.

•	Given the provided data, what are three conclusions that we can draw about crowdfunding campaigns?
We can conclude that most of the donors reached or exceeded their funding goal. Most of the donations come from plays with the least coming from world music. January has the highest number of failed donations across all platforms and years. The parent category with the highest amount of failed donations is theatre, which has almost twice as many failures as the 2nd and 3rd highest parent categories with failures in film & video and music. US has more successful donations than all other countries combined.

•	What are some limitations of this dataset?
The units of currency are not universal. It also does not cover all possible countries. We also have blurbs about each donor which appear to be unique and do not appear to be categorical, so we may have difficulty developing further answers for why one donor may be more successful than another.


•	What are some other possible tables and/or graphs that we could create, and what additional value would they provide?
We could develop a pie chart for each failed parent category that would show the percentage of the goal that was donated to see if we can notice any patterns. We could also use a pivot table with a bar graph to show the aggregated average donation for each category and/or country  to see if we notice trends in the country’s average donation vs the category’s average donation.  We could also use a bar chart to show how many backers each country or category has out of all of the failed pledges. 
![image](https://github.com/MDCummings86/Crowdfunding/assets/126340452/c0bf0618-3d73-4775-8b5a-18f5a34bffa8)



Crowdfunding Goal Analysis

Create a new sheet with 8 columns:

*Goal

*Number Successful

*Number Failed

*Number Canceled

*Total Projects

*Percentage Successful

*Percentage Failed

*Percentage Canceled


In the Goal column, create 12 rows with the following headers:

*Less than 1000

*1000 to 4999

*5000 to 9999

*10000 to 14999

*15000 to 19999

*20000 to 24999

*25000 to 29999

*30000 to 34999

*35000 to 39999

*40000 to 44999

*45000 to 49999

*Greater than or equal to 50000


<img width="870" alt="image" src="https://github.com/MDCummings86/Crowdfunding/assets/126340452/964c8c91-b52f-44fc-aa3f-67556bc4e107">


*Using the COUNTIFS() formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the Number Successful, Number Failed, and Number Canceled columns with these data points.
*Add up each of the values in the Number Successful, Number Failed, and Number Canceled columns to populate the Total Projects column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.
*Create a line chart that graphs the relationship between a goal amount and its chances of success, failure, or cancellation.

Statistical Analysis

Most people would use the number of campaign backers to assess the success of a crowdfunding campaign. Creating a summary statistics table is one of the most efficient ways that data scientists can characterize quantitative metrics, such as the number of campaign backers.
For gaining an in-depth understanding of campaign backers, evaluate the number of backers of successful and unsuccessful campaigns by creating your own summary statistics table.
Create a new worksheet in your workbook, and create one column for the number of backers of successful campaigns and one column for unsuccessful campaigns.

<img width="695" alt="image" src="https://github.com/MDCummings86/Crowdfunding/assets/126340452/86f0fa90-865c-4dca-b5ab-380efdcb272e">


Use Excel to evaluate the following values for successful campaigns, and then do the same for unsuccessful campaigns:

*The mean number of backers

*The median number of backers

*The minimum number of backers

*The maximum number of backers

*The variance of the number of backers

*The standard deviation of the number of backers

*Use your data to determine whether the mean or the median better summarizes the data.

*Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?
