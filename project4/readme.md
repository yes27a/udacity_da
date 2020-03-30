# Ford GoBike System Data
## by Eunsuk Ye


## Dataset

This is individual bike trip information made in a bike sharing system located in the greater San Francisco Bay area. Each trip data includes 15 columns which are trip duration in seconds, start date/time, end date/time, start station ID/name/geospatial info, end station ID/name/geospatial info, user type and bike ID. It is provided from this link(https://www.lyft.com/bikes/bay-wheels/system-data). This is originally very cleaned and only I removed 2 outliers of duration which is impossible in real. So Total data rows is little more than 5 milion. Additionaly I have extracted time-related information and additional trip-related type information from the exist features and created several new columns. Most columns are categorical variables in this dataset so I always use catplot function for visualization.



## Summary of Findings

In this exploratory data analysis, I have 3 kind of trip-related type such as duration type, trip type and user type. Duration type has short trip which is less than 30 min, mid trip which is 30 min-1.5 hour and long trip which is longer than 1.5 hour depends on the duration(I assume it is longer distance trip if the duration time is higher). Trip type has s1 type means trip returned to the start station and s2 type means trip ended another station than start. User type has subscriber and customer(casual user).
Most subscriber uses bike for work commuting during weekday and these trips are short trip and extremely high usage amount than any other time or usage of mid/long trip. Casual user also ride bike for work commute as well but the usage amount is very less than subscribers. It is very low usage amount though it looks like casual user constantly rides mid or long trip during both weekday and weekend. Their mid/long trip proportion is higher than subsciber's proportion. 
S1 trip proportion is extremely small amount means most people do not use returned trip so I think s1 type is not main factor of trend. 
This data contains 2017 through 2020. Bike riding is increasing over time for both subscriber and casual user. Spring, summer and fall is good weather for bike riding so this seasonal trend also observed for both user type. These increasing and seasonal trend is shown cleary in the short trip usage because of high amount however it is shown weak for mid/long trip usage. Peak usage time is during work commuting time. Daylight time riding during both weekday and weekend also was made but it seems a forth or less than peak usage amount.


## Key Insights for Presentation

In the presentation I focused on the short trip was made with super number and it shows increasing and seasonal pattern. But I was also noted that mid or long trip usage also was made constantly even they are super small number and it exist especially higher proportion in casual user's trip than subscriber's. Mid/long trip are also increasing over time and seasonally changed but I can say it influence weaker. Longer distance of trip, less influenced by season(weather) or week time(weekday or weekend).


