# Excel Challenge: Charting Crowdfunding
Used a database of 1,000 generated sample crowdfunding projects. Analyzed provided data to search for possible patterns and crafted conclusions based on the analysis.

1. First, I used conditional formatting in Excel to fill cells with a different color based on `Outcome`. I highlighted the failed campaigns in red, the successful campaigns in green, the canceled campaigns in yellow, and the live campaigns in blue.
2. Then, I created a column called `Percent Funded` that compared the actual funding to the initial funding goal and displayed the percentage of the initial funding goal that was obtained. I used conditional formatting to fill cells in `Percent Funded` in a three-color scale. I highlighted cells with a value equal to or more than 0 and less than 100 in dark red, cells with a value equal to or greater than 100 and below 200 in green, and cells with a value equal to or greater than 200 in blue.
3. I created a column called `Average Donation` to find how much each project backer paid on average. To obtain this, I looked at the acquired funding and divided it by the number of backers.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/Outcome_PercentFunded_AverageDonation.png)

4. I created a column called `Parent Category` and another one called `Sub-category` to split the contents of the `Category and Sub-Category` column into two separate columns.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/Category_Subcategory.png)

5. In another sheet, I created a pivot table to look at the number of campaigns that were failed, successful, canceled or live based on category. I created a stacked-column pivot chart that filtered the results by country based on the pivot table I created.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/CategoryStats_Pivot.png)

6. I created another sheet with a pivot table to analyze the outcome of campaigns per sub-category. Then, I created a stacked-column pivot chart that can be filtered by country and parent category based on the pivot table I created.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/SubcategoryStats_Pivot.png)

7. On the initial sheet I converted the `launched_at` and `deadline` columns from Unix timestamps to date format into two new columns `Date Created Conversion` and `Date Ended Conversion`. On another sheet, I created a pivot table that looked at outcome of campaigns and the date created, and filtered based on parent category and Years. I created a pivot-chart line graph to visualize the results.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/LaunchedDateOutcome_Pivot.png)

8. I created a new sheet that looked at the outcome of campaigns based on the crowdfunding goals. I created a table with a `Goal` column that specified the crowdfunding goal in ranges going from `Less than 1000` to `Greater than or equal to 50000`. The table showed the number of campaigns that were successful, failed, canceled, and the total number of campaigns in each crowdfunding goal range, and calculated the percentage of campaigns with each outcome. Then, I created a line graph based on that table to visualize the results.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/GoalOutcome_Pivot.png)

9. I created a new sheet that showed the successful campaigns and the number of backers, and on another column showed the failed campaigns and the number of backers. 
    - For successful campaigns, the `mean` number of backers was 851, the `median` was 201, the `minimum` was 16, the `maximum` was 7295, the `variance` was 1603374, and the `standard deviation` was 1266.
    - For failed campaigns, the `mean` number of backers was 586, the `median` was 115, the `minimum` was 0, the `maximum` was 6080, the `variance` was 921575, and the `standard deviation` was 960.
    - I concluded that the median summarizes the data better than the mean because outliers heavily skew the mean.
    - I also noted that there is more variability with successful campaigns, failed campaigns have a lower number of backers because these were campaigns that did not reach their crowdfunding goal, while successful campaigns exceeded their goal, increasing variability in the number of backers.
![alt text](https://github.com/glongo001/excel-challenge/blob/main/Images/Backers_Analysis.png)

10. In a Word document, I outlined my conclusions based on the Crowdfunding Campaign Data.
