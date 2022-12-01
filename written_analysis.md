# Kickstarter_Analysis
### Project Overview: 
To help Louise determine how campaign launch date and funding goal influence the success of a campaign. 

### Analysis: 
1. To determine the effect of campaign launch date on campaign success, a pivot table was created to display the number of successful/failed/cancelled campaigns based on month launch date
![Pivot Table_Theater Outcomes by Launch Date](https://user-images.githubusercontent.com/113721712/205153703-63f2b6b8-f35f-4b31-b0ce-5e5fc86f07e1.png)

To extract year based on 'Date Created', use the following formula: 
``` 
=YEAR([@[Date Created Conversion]])
```

2. To determine the effect of funding goal on campaign success, this required an additional table to be created. We counted the number of successful/failed/cancelled campaigns based on funding goal ranges (Less than 1000, 1000 to 4999, and so on). 
![Table_Outcomes Based on Goals](https://user-images.githubusercontent.com/113721712/205153854-f0dc1e4a-6273-4723-9f1f-3272b12ee4b5.png)

To count the number of successul/failed/cancelled campaigns by funding goal, the COUNTIF formula was used: 
```
=COUNTIFS(Kickstarter!$F:$F, "successful", Kickstarter!$D:$D, "<1000", Kickstarter!$R:$R, "plays")
```

3. Finally a pivot table was created to display the percentage of successful/failed/cancelled campaigns based on funding goals. 
![Pivot Table_Outcomes Based on Goals](https://user-images.githubusercontent.com/113721712/205154355-4a022d52-6a3d-4643-96a8-8e77101008db.png)

**Challenges:**
The line graph for "Outcomes Based on Goal" did not sort the x axis in the order I expected (from smallest to largest funding goal). I had to google how to do a manual sort option to make sure the funding goals displayed in the correct order on the line graph. 
![Challenge_Screenshot 1](https://user-images.githubusercontent.com/113721712/205155113-76a709c8-d420-4a8b-83f1-3b88d63148f6.png)
![Challenge_Screenshot 2](https://user-images.githubusercontent.com/113721712/205155122-77619158-522f-44e5-b6aa-e51ae5b62501.png)


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
