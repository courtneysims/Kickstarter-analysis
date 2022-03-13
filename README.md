# An Analysis of Kickstarter Campaigns
 

## Overview of Project

Louise’s play, Fever, came close to meeting its funding goal in a short amount of time. By examining the Kickstarter dataset, we can get a better grasp of how the launch date and funding goals affect a campaign’s success or failure. These trends for the campaign outcomes can give Louise a better understanding to strategically plan any future Kickstarter campaigns. 
	

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Within Excel, we can organize the data and summarize it using relevant filters into a pivot table to create a pivot chart, visualizing the data for better representation of the trends on the outcomes of a campaign. The pivot chart was created by filtering the Kickstarter campaigns to the theater genre and organizing the table by creating rows reflecting the launch date (as months) and columns reflecting the outcome potentials (successful, failed, and canceled). 

 **Pivot Table** 

![Pivot Table](https://github.com/courtneysims/Kickstarter-analysis/blob/691b924c525d04cda1eddb352f296800ec0c7053/Resources/Pivot%20Table.png)

In reviewing the pivot chart, it is evident that certain times of the year have a different tendency for the outcomes of the campaigns. 





 **Pivot Chart**
 ![Theater Outcomes Based on Launch Date](https://github.com/courtneysims/Kickstarter-analysis/blob/4926b5e5ad112b998379a7d59f1a21b4dcf22757/Resources/Theater_Outcomes_vs_Launch.png)


This is evident by the peak in most successful outcomes happening at the start of summer, particularly the month of May. The peak in failed campaign outcomes is reflected in the time of the year following the onset of the major holidays, particularly October. Interestingly, the trend following failed campaigns mirrors that of the successful campaigns, at a lower level. This could be reflected as a natural occurrence relating to the time of year. As there is a larger number of campaigns kickstarting at these times, a larger number of failed outcomes may also be reflected.   

A challenge for the pivot table and the chart is a possible shortcoming in not reflecting the reason for a campaign’s failed or canceled outcome. The successful campaigns seem to follow peaks in seasons, reflecting the population’s increased activity in the warmer months of summer where greater interest may be in seeking out and attending theater plays. A large peak of failed campaigns in the winter months may reveal another factor for the population by indicating disinterest in theater plays in competition with the holiday season. 

### Analysis of Outcomes Based on Goals

The data reveals more interesting trends when looking at the campaign outcomes in relation to the funding goal. To create the data for outcomes based on funding goals a reference column was created of funding ranges at 5,000 dollar increments. The number of each outcome type (successful, failed, and canceled) are represented in their respective column at each goal amount bracket. A difficulty I encountered was in correctly assigning the necessary ranges to satisfy the criteria for the COUNTIFS formula **(1)**. A quick write-out of the summary of what the formula needed to accomplish resolved my initial uncertainty. The formula needed to count the subcategory of “plays” that was of the outcome currently investigated within the funding goal range specified for that row. The resultant base formula accounted for my criteria and is flexible enough to be edited for the different outcomes and goals.  


=COUNTIFS(Kickstarter!$D:$D, "<1000",Kickstarter!$F:$F, "successful",Kickstarter!$R:$R, "plays")                                                             **(1)**


To further analyze the outcomes based on goals the percentage of each outcome for every funding bracket was also created, providing a quick comparison of trends as funding amounts increase. The higher percentages of successful campaigns seemed to reflect a turning point around the 20,000 dollar goal amount with the most being successful with a funding goal of 5,000 or less. After this point, as funding goals increased in their amount, the number of failed campaigns also starts to increase. The Kickstarter campaigns with a funding goal of over 45,000 performed the worst, having an 88% or greater chance of failure. The line graph below illustrates a close mirroring of successful versus failed outcomes, suggesting that factors other than the goal amount influence the outcome of a campaign.   


 ![Oucomes Based on Goals](https://github.com/courtneysims/Kickstarter-analysis/blob/4926b5e5ad112b998379a7d59f1a21b4dcf22757/Resources/Outcomes_Vs_Goals.png)
	

## Results

### Conclusions About Analysis of Outcomes Based on Launch Date

The dataset for these Kickstarter campaigns reveals several conclusions that can be made about the trends in outcomes. First, the time of the year plays an important role in the likelihood of a successful campaign outcome. This does make sense when viewing this data as a reflection of the population’s tendencies throughout the year. During the warmer months, people will be more active in public settings and seek more forms of entertainment such as attending a theater Kickstarter campaign. Conversely, during the holiday season, the population may have a reservation in spending and thus have more reluctance in considering funding a Kickstarter campaign. Therefore, Louise would be best served in planning the launch of a campaign that will take advantage of the population’s activity and spending tendencies. For this instance, the best month would be May, following the peak of the trend for backer interest and avoiding the competition that the major holidays would cause towards the end of the year. Also, a campaign remaining open through July may provide the best window for generating the most funds. A stacked bar graph would prove beneficial in visualizing the proportions of successful to failed outcomes for each month. The line graph in figure 1.2 showed clear peaks in successful campaign outcomes but also shows failed outcomes that mirrored to a lesser degree the same trend. The stacked feature of this type of bar graph would give Louise another level of information to further plan a successful Kickstarter campaign. 

### Conclusions About Analysis of Outcomes Based on Goals
When adding the inferences from the outcomes based on goals, Kickstarter campaigns with lower funding goals were more successful. In the future, a funding limit of 5,000 is advisable for the best chance of success. The sharp change in percentages for the goal amounts of 35,000 to 45,000 suggests that these funding brackets are possible outliers. The percentage of success does increase for this range but drastically falls following the funding bracket. A limitation of the dataset is not being able to further break down the cause of the outliers. Although the campaigns showed a successful overall percentage with a high funding goal, the surrounding brackets suggest this amount is still an unfeasible goal for most Kickstarter campaigns. It could suggest that certain types of Kickstarter campaigns may attract different tiers of backers with different funding abilities. The line graph for outcomes based on goals shows a drastic comparison of successful vs failed campaigns. This indicates that the funding amount is an important consideration when planning a Kickstarter campaign. Another element that may prove to be insightful is to analyze the demographics of the backers for each campaign. This would give Louise a better picture of her target audience and whether the expected funding goal is attainable or needs to be adjusted. 


### Data Used
Excel workbook: [Kickstarter_Challenge](https://github.com/courtneysims/Kickstarter-analysis/blob/4926b5e5ad112b998379a7d59f1a21b4dcf22757/Kickstarter_Challenge_Copy.zip)

