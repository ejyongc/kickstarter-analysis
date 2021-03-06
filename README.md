# An Analysis of Kickstarter Campaigns
Performed analysis on kickstart data to identify trends and make recommendations.  

# Kickstarting with Excel

## Overview of Project
After coming very close to hitting her Kickstarter goal, Louise sparked an interested to learn more about the different outcomes of the theater kickstarter campaigns in relation to their launch date and goal size. 
In this project we analyze Kickstarter data with the goal to visualize the three different outcomes (successful, failed, and cancelled) of the campaigns in relation to the month they were launched in and their goal size.  

### Purpose
The purpose of this report is to help Louise determine when would be the best time of the year to launch a successful kickstarter campaign, as well as setting an attainable campaign goal based on other campaigns data.   

## Analysis and Challenges
The analysis of the kickstarter data was divided into two separate sections: 
1. [Theater Outcomes by Launch Date.](###Analysis-of-Outcomes-Based-on-Launch-Date)
2. [Outcomes Based Goals.](###Analysis-of-Outcomes-Based-on-Goals)
    
### Analysis of Outcomes Based on Launch Date
In the first analysis, we pivoted the data to show the three different campaign outcomes (successful, failed, and cancelled) for all *Theater* Kickstart campaigns against their launch date. 

Our first challenge came when pivoting the table by month. First, we had to group the launch date field and then sort it in descending order. When we applied the pivot table filters it wouldn't sort them by month due to the fact that we are working with eight years of data. We ended up having to sort the months manually. 

Once the pivot table data was populated, we inserted a line pivot chart in order to visualize the data in chronological order. From this data we immediately identified a peak in successful theater campaigns during the month of May. 

![image](https://github.com/ejyongc/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

Finally, we wanted to identify if we had any outliers on our dataset. We ran a statistical analysis to determine if there were any outliers on the amount outcomes per month. (*Box and Wiskers* chart below)

![image](https://github.com/ejyongc/kickstarter-analysis/blob/main/Total%20Outcomes%20per%20Month%20-%20Statistical%20Analysis%20-%20Box%20and%20Wisker.png) 

### Analysis of Outcomes Based on Goals
In the second analysis, we segmented the campaign goals into 12 different ranges. We arranged the goals ranges to go from *"less than $1,000" to Greater than $50,000. 

We utilized COUNTIFS formulas to sort the data and determine the number of *successful, failed, and canceled* for each goal range. After that, we calculated the total SUM of all campaigns by goal range. 

After calculating the outcomes for each goal range, we ran the function SUM to add the total of projects by goal bracket. With this new data, we calculated the percentage of *successful, failed, and canceled* outcomes for each goal bracket. 

Finally, we calculated the percentage of *successful, failed, and canceled* campaigns by goal bracket and created a line chart to visualize the Outcome by based goal percentages. 

![image](https://github.com/ejyongc/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png) 

### Challenges and Difficulties Encountered

The first challenge that we came across in this analysis is that we are analyzing the subcategory "plays" while on the previous analysis we reviewed the parent category "Theaters". This approach could throw the result off since we are omiting some of the theater sub-categories like "musical" and "spaces".

## Results

#### - What are two conclusions you can draw about the Outcomes based on Launch Date?
1. The first conclusion we can draw from this analysis, is that based on the last 8 years, the month of *May* is the best time to launch new *Theater* kickstarter campaigns. 
2. The second conclusion from the analysis is that although *October* is the only month that has no *canceled* campaigns, there's a high number of *failed* campaigns in relation to the amount of *successful* campaigns during that month. 
    
#### - What can you conclude about the Outcomes based on Goals?
From the outcomes based on goals analysis, we can conclude that *play* campaigns with goals between $15,000 and $34,999 are more likely to fail. On the low end, *play* campaigns goals between $1 and $14,999 are more likely to be successful. On the high end, *play* campaign goals ranging from $35,000 and $44,999 are also more likely to be successful. In this case, depending on the goal size, we'd recommend Louise to launch campaigns based on those brackets. 

#### - What are some limitations of this dataset?
Some of the limitations of this dataset could be the external factors that could influence the success of these Kickstart campaigns. (For example economic changes, popular preference shift, etc). 

#### - What are some other possible tables and/or graphs that we could create?
Since we are analyzing the *Theater* category, it could be helpful to analyze the outcome of their sub-categories. Below is an example of what a bar char could look like. 

![image](https://github.com/ejyongc/kickstarter-analysis/blob/main/Theater%20Outcomes%20by%20Subcategory.png)
