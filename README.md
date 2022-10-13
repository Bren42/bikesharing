## Bikesharing Analysis

### Overview
The purpose of this analysis was to gather information including gender, age, location, usage, trip duration and more so that we could look at real data from a succesful bike share program in NYC and present to investors a plan to open a similar program in other areas. To do this we gathered the public data shared from the CitiBike program in New York and put some analysis into Tableau to show everyone what we found.

### Results

To start with we had to grab the CSV file and edit the tripduration field, we did this by pulling the data into PANDAS and creating a dataframe to complete the conversion.

Initial DataFrame creation 
![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/df_creation.png)

Checking DF types
![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/check_df_types.png)

convert the integer into a datetime object
![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/convert_int_datetime.png)

Create the CSV to be used in Tableau
![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/new_csv.png)

After converting the data into a format that we could use we began the analysis of the bikesharing program.

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/tripduration.png)
1.Trip Duration shows that almost all rides are less than an hour, with a median duration of 30 minutes. Meaning we could base fleet needs on this.


![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/tripduration_gender.png)
2. Checkout time by Gender is also a trip duration calculation however it shows us that although duration does not change much by gender, total ridership is much higher with male clients.

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/trips%20by%20age.png)
3. Trips by age is giving us a target age audience to market this to. From what we can see in the dashboard we have the bulk of clients in the age range of 25-40. there is an odd spike in ridership in the 52-54 age range as well but further analysis would be needed to determine why this spike exists.

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/trips_per_WDH.png)
4.Trips per weekday hour gives us two very critical data vectors, which day of the week is the most popular for riders and at what time. Many might assume that the weekend would be more popular, but as we can see weekday mornings around 8am, Thursday in particular, and weekday evenings between 5-7. This shows that we likely have  lot of residents who use the service to go to and from an office.

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/trips_per_Gender.png)
5.We can also look at trips per weekday hour and add the gender element to see if this tells us anything. As we can see Male clients contribute the most to the weekday morning and evening trends.

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/trips_per_usertype.png)
6. One of the last elements of the trips by weekday is the volume of customers versus subscribers. This shows a clear trend towards subscription based services. 

![This is an image](https://github.com/Bren42/bikesharing/blob/main/images/station_by_type.png)
7. Station usage by usertype allows us to see the most used stations and whether they are more frequently used by customers or subscribers, as in the prior data we see subscribers being the vast majoriy. However with more data we could look into the customer hotspots and determine why those areas are more likely to be used by customers.

For a view of the dashboard live please use the link below.
[Link to Dashboard](https://public.tableau.com/app/profile/brendon3165/viz/CitiBike_Challenge_16656914621650/CitibikeStory)

###Summary

In summation we can see that tableau does a great job of showing us a clear trend in usage patterns. In this case we would assume that we would want to market towards a 25-35 year old male who would be likely to pay a subscription for a pick up and ride service. 

