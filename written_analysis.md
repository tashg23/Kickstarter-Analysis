# Kickstarter_Analysis
### Project Overview: 
To help Louise determine how campaign launch date and funding goal influence the success of a campaign. 

### Analysis: 
1. To determine the effect of campaign launch date on campaign success, a pivot table was created to display the number of successful/failed/cancelled campaigns based on month launch date
2. To determine the effect of funding goal on campaign success, this required an additional table to be created. We counted the number of successful/failed/cancelled campaigns based on funding goal ranges (Less than 1000, 1000 to 4999, and so on). 
3. Excerpt of countif code 
4. Finally a pivot table was created to display the percentage of successful/failed/cancelled campaigns based on funding goals. 

**Challenges:**
The line graph for "Outcomes Based on Goal" did not sort the x axis in the order I expected (from smallest to largest funding goal). I had to google how to do a manual sort option to make sure the funding goals displayed in the correct order on the line graph. 

### **Results:** 
- Campaigns launching in May or June have the highest number of successful campaigns 
- Campaigns launching in December seem to have the lowest rate of success 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/113721712/205153149-c4cbc9bc-3ca3-43bc-b54e-45dc3313a01d.png)

- Campaigns with a large funding goal have lower success rates 
- ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/113721712/205153180-8b520aa6-64e9-4b49-a43e-612dbf8fa359.png)

**Limitations:**
The dataset doesn't provide any information on how the campaign was marketed. For example, some campaigns could have advertised their fundraising efforts using social media while others might not have. Different marketing tactics could lead to different rates of success. 

**Other possible analyses:**
We could look at whether the duration of the campaign has an effect on campaign success, which would involve creating another column (date created - date ended). We could look at whether campaign success is also influenced by other factors such as country. It might also be worth looking at the failed campaigns - if some campaigns were only a few hundred dollars away from their funding goal, then maybe it is worth classifying this group into a separate category, if they were still able to carry out their project with the funds they had. 
