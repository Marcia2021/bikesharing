# Bike-sharing Analysis Using Tableau

## Overview 

Tableau is one of the most popular data visualization tools. It can be used to transform the data into an engaging story for any audience. In this module we used Tableau to create worksheets, dashboards and stories to visualize key data from a New York Citi Bike dataset to present a business proposal for a bike-sharing company. 

In this analysis, we focused on August 2019 data in New York City, Des Moines. We were able to use Tableau to answer few research questions, such as how many bike trips were recorded during the month of August in the city of Des Moines, the number of short-term customers and annual subscribers to the Citi Bike service which help us determine the types of customers we could expect for a bike-sharing company in Des Moines, etc. Additionally, we are going to create more visualizations for the following subjects:

-	Length of time that bikes are checked out for all riders and by gender.
-	Number of bike trips for all riders and genders for each hour of each day of the week.
-	Number of bike trips for each type of users and gender for each day of the week.

## Analysis

1.	In the original data, “tripduration” is an integer. In order to analyze the Citi Bike data by hour, used Python Pandas to_datetime() function to convert “tripduration” to a     datetime datatype in hours, minutes and seconds. 

    ![inst1](https://user-images.githubusercontent.com/79289806/120207999-0b91f900-c1fb-11eb-996c-c85300416bb0.png)

    Exported the new data to CSV without index.

    ![inst2](https://user-images.githubusercontent.com/79289806/120208001-0b91f900-c1fb-11eb-8088-83b8582bffb7.png)

2.	Used Tableau to create visualizations. 

## Results

[link to CitiBike Trip Analysis Tableau Story](https://public.tableau.com/app/profile/miaomiao.shen/viz/NYCCitiBikeAnalysis_16226726258510/Story1)

1.	After converted “tripduration” to datetime datatype:

    Before conversion:

    ![inst3](https://user-images.githubusercontent.com/79289806/120208340-5dd31a00-c1fb-11eb-9ec5-64d874a92b2d.png)

    After conversion:
 
    ![inst4](https://user-images.githubusercontent.com/79289806/120208343-5dd31a00-c1fb-11eb-9a33-28e493cc1f28.png)

2.	Total number of records in August 2019 Citi Bike data in the city of Des Moines:

    ![vis01](https://user-images.githubusercontent.com/79289806/120207748-cd94d500-c1fa-11eb-91a0-e101546f0e34.png)

3.	Checkout Times for all users: 

    ![vis1](https://user-images.githubusercontent.com/79289806/120207749-ce2d6b80-c1fa-11eb-8900-69a39bdb218e.png)

    This line chart could be filtered by the hour of trip duration. The peak of bike trip duration appears at 0 hour 5 mins. 

    There are total of 2,344,224 rides in the city of Des Moines in August 2019, 146,752 of them checked out in 5 mins, which is 6.26% of the total rides. 

4.	Checkout Times for all users by Gender:

    ![vis2](https://user-images.githubusercontent.com/79289806/120207750-ce2d6b80-c1fa-11eb-9295-a6b154286bf3.png)

    Similar as the line hart for all users, this chart analyzed the bike sharing data by Gender that could be filtered by the hour of trip duration. 

    Among all the riders that checked out in 5 mins, majority of them were male (108,087), which is 73.65% of these users.  

5.	August peak Hours in all users: among all users the peak hour of bike usage is at 8am and 4pm to 7pm regardless of user type.

    ![vis03](https://user-images.githubusercontent.com/79289806/120207751-ce2d6b80-c1fa-11eb-8200-b6815be66716.png)

6.	Trips by Weekday per Hour: this heatmap shows the number of bike trips by weekday for each hour of the day.

    ![vis3](https://user-images.githubusercontent.com/79289806/120207752-ce2d6b80-c1fa-11eb-887d-5ce06a8cfe5b.png)

    From this graph, we could see that there are two peaks:

    - 	Monday, Tuesday, Thursday from 5pm to 6pm.
    - 	Monday to Friday at 8am.

    In the weekdays, these are the rush hours for commuters. This might mean that in big cities like NYC Des Moines people are more likely to choose bike as transportation to       work when weather allows. 

    Additionally, during the weekend, 10am to 7pm have a higher rate of bike usage compared to other times. This might due to the bike usage of customers. 

7.	Trips by Weekday per Hour by Gender:

    ![vis4](https://user-images.githubusercontent.com/79289806/120207754-ce2d6b80-c1fa-11eb-80f5-d0a4786eba74.png)

    This heatmap shows consistent information as the previous graphs. Male has higher usage of bike than Female. The peak of bike trip is consistent as the peak in all users. 

8.	User Trips by Gender by Weekday:

    ![vis5](https://user-images.githubusercontent.com/79289806/120207755-ce2d6b80-c1fa-11eb-82ff-a6b9509b0a68.png)

    Among all the users, subscriber has higher number of bike trips compared to customer. Among subscriber, male has higher number of bike trips compared to female. Among           customers, weekends have a slightly higher number of bike usage compared to weekdays. 

9.	Created Story with the graphs created from previous steps to better present the data to investors:

    ![v6](https://user-images.githubusercontent.com/79289806/120207756-cec60200-c1fa-11eb-9718-66c31c07cdc9.png)     

## Summary

In NYC Des Moines, there is a high activity of bike sharing service during August 2019. Among all the users, male subscribers have higher number of bike usage compared to other users. The peak hours of bike trips happened during the rush hours in the morning and afternoon in weekdays, which indicates that in big cities, such as the city of Des Moines, bike might be a popular public transportation for commuters. Additionally, when the weather getting better, bike might be one of the popular cities visiting method among customers.

There are more graphs we could create from the data to better help the decision maker:

-	User Trips by Weekday per Hour, which will help us to confirm the higher usage of bike for subscriber during the weekdays, and higher usage of bike for customers (might be       majority of tourists) during the weekends.

-	Since this analysis only focused on August 2019 data, we might able to get the whole year bike trip sharing data to analyze the trend of bike usage across the year. 
