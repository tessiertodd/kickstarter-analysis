# Kickstarter Campaign Overview #

## Overview of Project: ##
The objective of this project is to provide insight to our client (Louise) on the factors driving the successes and challenges of other Kickstarter projects.


## Purpose: ##
Client is looking to fund a play through Kickstarter and wants to understand other Kickstarter projects to help ensure she is able to run a successful fundraising campaign.


## Analysis and Challenges: ##

### Analysis of Outcomes Based on Launch Date ###
Launching a Kickstarter campaign in May for a play is the ideal month as there is over 2x more successful launches in May than failures.  May is also the month where the most Kickstarter projects are launched.

![Table_Launch_Date](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Table_Launch_Date.png)
![Theater_Outcomes_vs_Launch](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals ###
The most successful outcomes based on goals are those that are less than $5,000 (2 groups included with less than $1,000 slightly higher) with over 70% success rate.  A key challenge is those are really small budgets to put on a play.  At a higher budget, the most successful goals are $35,000 to $45,000 (2 groups included as both very similar success rate) at just over 66% success.

![Table_Goals](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Table_Goals.png)
![Outcomes_vs_Goals](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered ###
**Outcomes Based on Launch Date** – not so much a challenge, but interesting learning that even through I selected a date column (Date Created Conversion) that was an actual date, the pivot table put in year, quarter and month… but not the actual date.  That was helpful, but also interesting.  I just moved the year and quarter out as I only needed to see month.

![Original](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Date_pivot_interesting.png)
![Changed](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Date_pivot_change.png)

**Outcomes Based on Goals** - while I had used SUMIFS in the past, I had not used COUNTIFS… but approach the same.  At first, I had assumed I could only have two sets of criteria so was not sure how to filter on plays and get into the right grouping of number of successes so I had taken an alternate approach (tab: “Outcomes Based on Goals v2” which is hidden).

![Goal_learning](https://github.com/tessiertodd/kickstarter-analysis/blob/main/Goal_learning.png)


**Other challenges** – the parent category “theater” (used in Outcomes Based on Launch Date) and sub-category “plays” (used in Outcomes Based on Goals) are both still pretty broad – we may want to look at further segmentations to help client get even more relevant insight about their specific play (ie. type of play, country, number of backers).  One other challenge that may change some of the groupings in Outcomes Based on Goals is the currency (different currencies in different countries)… typically important when comparing financial information that different currencies are translated to one for comparability.


## Results: ##
What are two conclusions you can draw about the Outcomes based on Launch Date?
•	Launching a campaign in May is where we see the highest opportunity for success (over 2x the number of failed campaigns) ... also the month where most campaigns are launched.
•	December is when the least amount of theatre campaigns are launched... and where success and failure are very closely aligned.

### What can you conclude about the Outcomes based on Goals? ###
•	The change of success is higher at lower levels of goals in general than higher... below 20,000 success rate is higher than failure rate.  The exception is from $35,000 to $44,999 there is a higher chance of success than failure.  Very high campaigns $45,000+ have a very high chance of failure (over 80%).
•	Interesting that there were no plays campaigns cancelled... we did in other sub-categories.

### What are some limitations of this dataset? ###
•	Goal and Pledged as in different currencies... could lead to some different conclusions for example when looking at Outcomes Based on Goals.
•	Categorization does not split out "plays further" (sub-categories not split out further), which could provide more insight specific to a particular type of play that Louise is looking to put on (ie. drama, comedy).
•	There is no description of success of actual event (ie. did play get rave reviews and/or sell many tickets)
•	No insight into the amount or type of advertising done for each project.

### What are some other possible tables and/or graphs that we could create? ###
•	Number of backers and average donation for those plays in a particular country... possibly understanding of how many backers you would need or target.
•	Look at impact of Staff Pick or Spotlight on success/failure.


## Recommendation: ##
I would recommend that client look to launch the campaign for the play in May with an objective between $30,000 to $44,999 (providing budget required is in that range) to help improve the chance for success with the campaign while ensure that the play is properly funded and is a positive project.
