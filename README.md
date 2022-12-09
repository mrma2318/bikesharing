# Bike Sharing
[Citi Bike Sharing](https://public.tableau.com/app/profile/morgan.anderson5677/viz/CitiBikeSharing_16705475515210/CitiBikeSharing)

## Overview: Analyzing Citi Bike data from New York City as it applies to Des Moines.
### The purpose of this analysis is to solidify a propsoal showing the length of time that bikes are checked out for all riders and genders, the number of bike trips for all riders and genders for each hour of each day of the week, and for each type of user and gender for each day of the week.

## Analysis
- Before I could start analyzing the data, I needed to know what questions to ask and what my audience is looking for. Therefore, the first questions was to answer how many bike trips were recorded during the month of August so we knew how many rides to expect in Des Moines during that time. To find out the answer to this question, I just needed to drag my citi data to the text box in marks. The worksheet then updated with the number of rides: 2,344,224 rides.

- Next I wanted to get the breakdown of gender. It's important to understand who our riders are themselves. Therefore, I created a pie chart, Image 1, to help us learn a little more about the customers. 

### Image 1: Gender Breakdown
![Pie Chart](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/GenderBreakdown.png)

- Then I wanted to understand the length of time that bikes are checked out as well as checked out for each gender. To visualize this information in Tableau I had to add the number of records for the rows, and the tripduration to the columns. In addition, I needed to make sure to change the filter for tripduration to hour. However, I also wanted the minutes, so I had to add tripduration again to the columns and filter that one by minutes, and change the value to be continuous. Then to include the checkout times by gender, I put gender as a color in the marks field.

- Now that we know that August is a good month to visit the city, knowing the peak hours for bike trips during the month will also be important. Knowing this information will also help provide an estimate of how many bikes we might need, as well as which parts of the day we'll need the most bikes. Understanding the checkout times, will also assist in estimating how many bikes we need. This visualization is best using a bar graph, Image 2. I put the start time dimension into the rows section, and then changed the "year" to "hours" since we wanted to find peak hours. Then, I added the citi bike data to the columns and changed the measure to "sum".

### Image 2: August Peak Hours
![August Peak Hours](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/AugustPeakHours.png)

- Understanding high traffic locations is also important in both when and where people are using Citi Bike. Therefore, we want to find the most popular stations in the city for starting a bike trip. First I had to add the start station longitude measure to the columns section and the start station latitude to the rows section. Then I needed to change the measures to dimension. In the marks sections, I also changed "automatic" to "map". I also want the most popular starting locations to have a different size and darker color to represent the popularity of that location. To adjust the size of the symbol, I had to add the citi bike data to the size button in the marks section. To adjust the colors to help differentiate between the most popular locations and less, I also had to add the citi bike data to color in the marks section, Image 3. 

### Image 3: Top Starting Locations
![Top Starting Locations](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/TopStartingLocations.png)

- Next, I wanted to create a visualization with a heatmap that shows the number of bike trips broken down by gender by each day of the week by each Usertype. Therefore, I used the converted column for gender and added it to the columns. Then I added the Usertype to the rows, as well as the start time to the rows and changed the option to Weekday. I also needed to make sure I changed the marks field to automatic to create the heatmap.

- Lastly, I wanted to create visualizations of the trips by weekday for each hour, as well as by gender as a heatmap. First, I added the start time column to the rows and then filtered by hour. Then I added the stop time to the columns and filtered by weekday. I added the number of records to color in the marks field and selected automatic for the type of graph to create the heatmap like I did on the previous visualization, Image 4. To add the gender to the heatmap, I put the gender in columns.

### Image 4: Trips by Weekday For Each Hour
![Trips by Weekday for Each Hour](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/TripsByWeekday.png)

## Results
- The pie chart shows the gender breakdown of the customers and subscribers that use Citi Bike. The chart indicates that about 65% of subscribers/customers are male, while about 25% of them are female. The remaining 10% gender are unknown. 

- The checkout times by gender graph indicates the length of time citi bikes are checked out for. From the graph you can see the males check out more bikes than other subscribers/customers. However, the duration of time the bikes are checked out, regardless of gender, appear to be around 47 minutes, Image 4.

### Image 5: Checkout Times by Gender
![Checkout Times by Gender](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/CheckoutTimesByGender.png)

- The top starting locations map shows the most popular stations in the city for starting a bike trip. When you hover over the symbols, the latitude and longitude will show, as well as how many bike trips started at that location. At this time, the latitude and longitude of the station with the highest starting location is (40.75, -73.98), with 16,546 bike trips starting at this location. 

- Since August is a good month for Citi Bike, the August peak hours chart, shows the peak hours for pike trips during the month. By looking at the chart, you can see the peak hour for bike riders is around 5pm to 7pm, Image 2.

- The User Trips by Gender By Weekday, shows the number of bike trips broken down by gender by each day of the week. As you can see from the map, Image 5, male and female subscribers take more bike trips on Thursdays and Fridays, whereas customers are more likely to take more bike trips on Saturday's. On Thursday, around 259,000 males take a bike trip, and about 88,000 females. There are more unknown customers than unknown subscribers, with unknown customers taking more bike trips, around 55,000, on Saturday. 

### Image 6: User Trips by Gender by Weekday
![User Trips by Gender by Weekday](https://github.com/mrma2318/bikesharing/blob/b2917466e0f618d705d65712fd22289ccdf638f2/images/UserTripsByGender.png)

- The Trips by Weekday for Each Hour graph shows the trips by weekday for each hour of the day. The heatmap provides information on peak times that trips are taken during the week for each hour of the day. As you can tell, most trips are taken on Thursdays between 5pm and 7pm, with around 89,000 bike trips happening within that timeframe. The Trips by Gender heatmap, shows the same as the Trips by Weekday, however, it's broken down by gender by weekday for each hour. This map allows you to see the difference between male, female, and unknown peak times during the weekday per hour. With around 62,000 out of the 88,000 bike riders from 5pm to 7pm are male, around 21,000 are female, and the remaining are unknown. 

## Summary
- Overall, there are more male bike riders than female, and the peak time for subscriber bike riders is on Thursdays anywhere between 5pm to 7pm. However, unknown gender customers have a higher peak time of riding bikes on Saturday around 12pm. To see the complete Tableau Story, you can visit [Citi Bike Sharing](https://public.tableau.com/app/profile/morgan.anderson5677/viz/CitiBikeSharing_16705475515210/CitiBikeSharing).

- A few additional visualizations that I could perform to provide additional results on the citi bike data for Des Moines is first to look at the most used end station. We wanted to know where the top starting location was to make sure we had enough bikes. Understanding the top end location can be beneficial as well, this way we know where most of the bikes end up. This then allows us to know where we can also pick up most of our bikes during the day. If for some reason the main starting location starts to run out of bikes, we know that in about an hour, most of the bikes will be at the top end station for pick up. This way, bikes can constantly be returned to the starting location for continous bike trips. This way, we don't ever run out of bikes at the top starting location by continously cycling the bikes through.

- Another visualization would be to look at additional summer and fall months. While August has great reportings of bike sharing, other months might have equally great reporting. By looking at months close to August, you can gather additional information on peak times subscribers and customers go on bike trips and other peak days of the week. Looking at the same information we gathered for the month of August, can also be beneficial to gather with the surrounding months such as July and September to compare. By gathering this information, you can gather the overall months that have peak bike sharing. 