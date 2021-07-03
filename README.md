# Kickstarting with Excel

## Overview of Project
We analyzed over 4000 Kickstarter campaigns from 21 countries to help our client best decide how to most effectively start her own campaign for her theater production. Looking at which campaigns met their goals and which did not we can advise her on how to best fundraise and market her play.
### Purpose
We analyzed the data to doscover how outcomes werw effected by a number of variables. We attempted to find the optimal time to start a successful fundraising campaign, as well as identify the range of fundraising goals that produced the most successful campaigns. 
## Analysis and Challenges
To accomplish our task, we viewed the data in a number of ways. Using Microsoft Excel we sorted and filtered the data using pivot tables, charts, and various filters. Initially breaking the data down by outcome and when the campaign was launched, we were able to see which months had the most successful, failed, or canceled campaigns. One tricky part of this analysis was figuring out how to disregard the live campaigns on the table, as they were incomplete and we only wanted data on completed or canceled campaigns. A simple filter of the outcomes got us by this problem. We will look at and analyze this data in the section titled "Analysis of Outcomes based on Launch Date" below.

Next we wanted to look at the Outcomes of various kickstarter campaigns based on their initial goal. We broke the data down by $5000 increments, counting the number of plays that were successful, failed, or canceled. We used the COUNTIFS function on excel to calculate these amounts. Getting the syntax of these functions was difficult as I had not used it before, but after practice it became easier. Here is an example of the function we used to count the number of succesful play campaigns from $1000 to $4999, "=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<4999",Kickstarter!$R:$R,"plays"). Then, we calculated the percentage of plays in each price range that were successful, failed, or canceled. A chart looking at this percentage data is listed below in a chart titled Goals vs Outcomes.

### Analysis of Outcomes Based on Launch Date
<img src=resources/Theater_Outcomes_vs_Launch.png>
Here we can see the successful, failed, and canceled outcomes based on the month each campaign was launched. We will discuss the conclusions that can be drawn from this data below.

### Analysis of Outcomes Based on Goals
<img src=resources/Outcome_vs_goals.png>

Here we can see the percentage of each Play campaign that was successful, failed, or canceled based on the range of its initial goal. There were no canceled play campaigns in these price ranges so we do not see a "canceled" line on our chart.

## Results

- From looking at the Outcomes vs Launch date data, we can see that by far the most successful months to launch a campaign were in May and June. We had over 100 successful campaigns in each month. We can also see that December and January were the worst months to start a campaign, with the lowest number of successful campaigns. 

- From the Outcomes vs Goals chart, we can draw a few conclusions. Our most successful campaigns had goals of less than $1000, from $1000 to $4999, and then from $45000 to $49999. The last group from $45000 to $49999 is a little misleading, as there was only one campaign in that price range so the sample size is not large enough to say that 100% of all Kickstarter Campaigns in that price range will be successful. The sample size of the lower ranges, >$1000 and from $1000 to $4999, have a large sample size and thus we can be more confident in the conclusion that roughly 75% of those campaigns were successful. Ideally Louise would target raising an amount of money in that range. We can also see from the graph that as the campaign goals rise from less than $1000 to $30000, the liklihood of meeting out goal decreases.

- The data is slightly limited in a few ways, but the way that stands out the most is that past a $15000 goal the sample size decreases significantly and thus the conclusions we draw may not play out in the real world the way the data would suggest. 

- We could use other graphs and charts to analyze the data to draw different conclusions and gain additional insight into the best way to run a Kickstarter Campaign to raise money for a play. By looking at the number of backers for each project vs launch date we can see when projects are more likley to get more individual contributions. We could also chart the average donation for each campaign and each project subcategory, to see which types of projects receive more donations than others. These are just two examples of different ways we can examine this data.