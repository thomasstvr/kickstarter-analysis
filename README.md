# Kickstarting Louise to Success
## An Overview
In this project we have utilized Excel to visualize the best plan of action to launch a successful Kickstarter campaign in the future. Data from past Kickstarter campaigns was sorted and plotted using pivot tables and charts in order to help Louise in her coming endeavor.
### Why, You Ask?
Louise’s play Fever came close to meeting its Kickstarter campaign goal but unfortunately was not successful. She has contracted us to show the success and failure of different campaigns in relation to both their launch date as well as their set goal. With this information, future Kickstarters will have a much better chance at funding their play with a successful campaign.
## Analysis and Challenges
In order to analyze the data set in which Louise was interested in, we had to first sort out all the unneeded information. Louise is interested in funding a play, not funding the launch of a food truck. Once this is done, we can begin to help Louise using the Kickstarter data.
### Outcomes Based on Launch Date
In order to analyze the outcomes based on launch date, we first created a pivot table in Excel. The table was then filtered by year and parent category (in which the theater category was the only one selected).

![Outcomes_vs_Launch_table.png]( https://github.com/thomasstvr/kickstarter-analysis/blob/main/Outcomes_vs_Launch_table.png)

Once the table has been made, we simply plotted the data using a stacked line pivot chart.

![]( https://github.com/thomasstvr/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Outcomes Based on Goals
Analyzing the outcomes based on goals is a little trickier since the numbers we need are not right in front of us, some calculations must first be made. What we want to look at is the percentage of Kickstarter campaigns (with a subcategory of plays) that were successful, failed or canceled based on their goal.
In order to do this, we used Excel’s COUNTIFS function to count only campaigns within a designated range that matched our previously stated criteria. We used this data to build a new table, then calculated the percentage of each range that were categorized as successful, failed, or canceled. 
![]( https://github.com/thomasstvr/kickstarter-analysis/blob/main/Outcomes_vs_goals_main_table.png)

From here, we were able to do just as we had done with the Outcomes Based on Launch Date. We built a pivot table with the set goal range as our rows and the percentage successful, failed and canceled as our values. A stacked line pivot plot was then generated from this table.

![]( https://github.com/thomasstvr/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
The analysis of this data set using Excel is not too difficult but there were some places where we got hung up and spent a little more time than we should have. Building the Outcomes Based on Goals table was tedious but nothing too cumbersome.
When creating a pivot plot, the field buttons are shown within the plot as dropdown menus. It took us a little while to figure out that you can hide them all by right clicking on one and selecting “Hide All Field Buttons on Chart”. Another problem which seemed take us too much time to figure out was how to manually sort the ranges in the Outcomes Based on Goals pivot table. When you sort using ascending or descending things get out of order because two of the ranges are not strictly number based. To manually sort the range, you right click the column then click sort and select Manual under the more options tab. The problem came when we tried to click and drag the cell to be sorted. The cursor must be placed at the edge of the selected cell, where the cursor turns into four arrows. This can be easily overlooked by moving the cursor around too quickly. 
## Results
Based on the data, the best month to launch a Kickstarter campaign in order to fund a play is May, the data almost seems to follow the weather. In the hotter months, there are much more successes than failures whereas in the colder months they begin to merge closer together. By launch date, December is by far the worst month to launch campaign. 
Looking at the Outcomes Based on Goals chart, we see that the smaller goals have a much higher chance of being successful. There is a mentionable divergence from this conclusion for goals ranging from $35,000 to $45,000 USD. In the US, there were only 8 campaigns with a goal in that range which is not a large enough pool to conclusively say that it would be a good idea to set a goal that high. It is recommended that Louise keep her goal under $5,000 where data points are plentiful and chances for success are much larger.
A few things this data set lacks are background of the people behind the campaigns and the amount of advertisement for each campaign. A famous playwright will always have a much higher success rate than someone who is unknown and looking to fund their first play. Also, the amount of advertisement a campaign gets would greatly influence its success or failure. A campaign that gets lots of shares on social media would be more likely to succeed than one that did not receive any shares at all.
Some other possible tables that could be created are tables based on location and tables based on the number of backers. What country is best suited to start a Kickstarter campaign to fund a play? Is it best to have a small handful of backers who largely contribute or many backers who each contribute little?
