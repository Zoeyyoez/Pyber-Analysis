### PyBer_Analysis

## Summary 

The purpose of this project is to 
    1. create a summary DataFrame of the key metrics for the ride-sharing data by city type; and 
    2. create a multiple-line graph that shows the total fares for each week by each city type. 

To acheive the two goals, pandas and matplotlib are applied as the main tools for the analysis. In the initial step, pd.read_csv is used to read the csv files and pd.merge is used for merge the two datasets. For the first technical deliverable, the groupby and sum function are beling applied for purpose of getting total rides, total drivers, and total fares for each city type. After calculated the total and average value for all metrics by each city type, we created a PyBer summary DataFrame that includes Total Rides, Toral Drivers, Total Fares, average Fare per Ride and Average Fare per Driver. The last step was to delete the indext name and formate the DataFrame by correcting Number format (adding dollar sign etc.). 

Following is the final result for Technical Delieverable 1: Get A Summary DataFrame 
-![Deliverable1](https://github.com/Zoeyyoez/Pyber-Analysis/blob/master/images/Deliverable1.png)

Base on the DataFrame, it is indicated that the larger the volume of total rides the more drivers and more total fares. However, the larger the volume of rider the lower the average fare per rider and average fare per driver. 
-![Deliverable2](https://github.com/Zoeyyoez/Pyber-Analysis/blob/master/images/Deliverable2.png)

To plot for the Technical Delierable 2, we used rename, set_index, drop and groupby function to reorganize the DataFrame, and applied matplotlib to generate the line graph to showcase the changes of fares from 1/6/2019 to 4/28/2019. The graph also demonstrates that the total fares in urban cities has even exceeded the sum of rural cities and suburban cities. 

## Challenge 

The biggest challenge for this project is to figure out how to remove the index for the DataFrame. By researching the issue, I found a couple solutions online including using del function or hide the index but none of these worked due to unknow reasons such as can't delete attribute etc. I finally found an instruction that suggest to assign df.index.name = None, and it has successfully print the DataFrame without index. 

## Recommendation 

As there are more drivers than rides in Urban cities, it is suggested to increase marketing reach to the riders promote the business. Similarly, to encourage more drivers to participate in the business would also balance the disparity between rides and drivers. 

For the future analysis, I would also cover the change of fares in different times in a day. For example, will the fare after 10p.m. be less expensive than the fares in the mornig rush hour? To do that, groupby will be used to group different timeslots and matplotlib can also be applied to generate the line chart. 
