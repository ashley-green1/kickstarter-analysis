# kickstarter-analysis
Performing analysis of Kickstarter data to uncover trends.

# Theatre Play Fundraising Campaign Analysis


## Overview of Project


### Background and Purpose


#### What is the Background?
Louise recently completed the fundraising campaign for her play, *Fever*, and would like to know how other campaigns performed in comparison. 

#### What is the End Goal?

Louise specifically wants to know who other campaigns performed based on launch date and goal amount. Working with the data I already secured when Louise planned her goal, I will report to Louise the best month to launch a campaign and the most successful goals. 


## Analysis and Challenges

#### Outcomes Based on Launch Date
The Outcomes Based on Launch Date analysis relied heavily of using Pivot Table. Following I will provide screenshots of the steps I took to get the visuals. 

Here are my Pivot Field Settings and the final Pivot Table.
![image_name]
  
Next, I created a PivotChart to visualize the data. 
 

I wanted more insight and did not want to distort my work so far, as it was required, so I then created a table using paste special values to get the data out of the pivot table. From there I calculated the Percent of each outcome by month. 

Here is the paste special values table. 

 



Next, I selected the Month, Successful and Successful% columns from the paste special values table and used the insert tab to create the following two charts.
    


#### Outcomes Based on Goals
The Outcomes Based on Goals analysis relied heavily of advanced formulas such as CountIFS, Logical Operators, and good Excel Modeling skills. Following I will provide screenshots of the steps I took to get the visuals. 

    


I went further in this analysis and included charts with statistics that would help understand campaign outcomes based on goals. This relied heavily of Name Ranges and Array Functions.

I first filtered on the kickstarter data to show the “plays” subcategory only, then pasted it into a new sheet called Play Goal Outcomes. I used this for the analysis.

The formulas for the statistics were:
-AverageIFS
-MEDIAN
-MODE.SNGL
-STDEV.P
-QUARTILE.EXC

I did make the Statistic Nicknames shown on the chart more friendly for an audience that doesn’t have a data background.

Here is a copy of the statistics table used to create the charts.
 


  

### Analysis of Outcomes Based on Launch Date


#### May is the Most Popular & Best Month to Launch a Campaign

 

A quick glance at the Theater Campaign Results by Month Launched chart reveals that May is the most popular month to launch a campaign.  A May launch date also yields the highest number of successful campaigns. 







  

Including total number of campaigns by month indicates that success could be higher for May simply because more campaigns were launched that month. It is important to note that ALL trends almost the same as Successful. In fact, both Successful and Failed campaigns are higher in May. This information leads me to believe that more than Month Launched influences the success of a campaign. 

Is the popularity of May skewing the data? I will dive further into this to uncover other influences, but for now I can only conclude that 1) May is the most popular month to launch a campaign and 2) there are other influences driving success.


 

Charting the campaign outcomes as a percentage of all campaigns launched by month helped to reveal the odds of each outcome.  In November, there were 54 Successful campaigns out of 88 total campaigns, yielding a 61% success rate. The odds of success range from 49%-67% with May being the highest and December the lowest. 

This is not a wide range, unfortunately, and my goal is to identify and confirm the best time to launch. 

Next, I compare the Success Odds by Month (%) to Success Count by Month for more insight.

  

Comparing Success Odds by Month (%) to Success Count by Month solidifies that there are influences driving success other than timing.

For example, despite November being an unpopular month, the success rate is 61%, which is higher in the success range noted earlier. However, November is the 2nd to last most popular month to launch a campaign. It is good to see this as it eliminates any skewed data from driving decisions.

I now additionally conclude that May, with a Success Rate of 67%, is the best month to launch a campaign. 


### Analysis of Outcomes Based on Goals
#### Success Declines as Goals Increase
 


Looking at Play outcomes by goal range has been very insightful. As expected, success declines as the goals increase and failure increases as the goals increase.  Unfortunately, due to the low number of campaigns with goals above $10,000, the success rate appears higher than it should for $35,000-49,999 and larger.

The following 2 charts provide helpful statistics regarding the average, most popular and ranges of goals and their influence on outcome. 
  


The Average Goal for Failed campaigns is more than 2 times higher than the it is for Successful campaigns. The same goes for the Most Popular Goal which is $2,000 for Successful and $5,000 for Failed. 

The Average Pledged for Successful campaigns is $4,536 while the Averaged Pledged for Failed Campaigns is $527.

It is clear that a campaign with a higher goals are more likely to fail to meet them. 


## Limitations of this Dataset

There are several limitations with this dataset though there is enough information within the kickstarter data to get the job done.

The instructions for this Deliverables 1 & 2 limited the analysis. For example, there were specific directions on criteria to filter for pivot tables and charts. None of which required filtering by country nor recent years. Had such filters been included in the instructions, it would increase the reliability of the data for the analysis. 

Outside of instructions limiting the analysis, here is some data missing from the kickstarter data that I wish were available:

-Was the campaign marketed outside of the platform? 
-How fast did campaigns reach their goals? Many exceeded their goal and remained live until the deadline. 
-




## Challenges and Difficulties Encountered

The challenge with preparing this analysis is that I am expected to satisfy Louise’s curiosity with charts that didn’t properly complete the picture.  While they did provide some information, it didn’t dig as deeply as I’d liked to be confident the analysis is complete. 


## Other Possible Tables and or Graphs

I’ve included several additional charts and graphs with my analysis. 
We could also include Average Campaign Length in Days. We could calculate Campaign Length by subtracting Launch Date from Date Ended.
