# Ford GoBike System 2019
Bay Wheels is a regional public bicycle sharing system in the San Francisco Bay Area, California operated by Motivate in a partnership with the Metropolitan Transportation Commission and the Bay Area Air Quality Management District. Bay Wheels is the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established as Bay Area Bike Share in August 2013. As of January 2018, the Bay Wheels system had over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose. On June 28, 2017, the system officially re-launched as Ford GoBike in a partnership with Ford Motor Company. After Motivate's acquisition by Lyft, the system was subsequently renamed to Bay Wheels in June 2019. The system is expected to expand to 7,000 bicycles around 540 stations in San Francisco, Oakland, Berkeley, Emeryville, and San Jose
# Overview
bay wheel records a lot of information about each trip like start and end coordinates ,duration of the trip ,when does it start and end and record the date time of the trip and information about user like user type which indicates if user is customer or subscriber . 
data looks pretty clean but it needs more assessing .I have assessed it and found that there are tidy issues like 
- wrong data type which is expected because excel can't predict the wright data type 
 and it doesn't support some data types like datetime and category data types.
- missing data in some columns ,this missing data are not stored in any dattset and it's impossible to predict it so the best solution is removing it.
- there are 30 rows has inaccurate start and end time ,the start time took a place after end time which doesn't make sense i have interchanged them 
- 30 negative value caused of the above reason ,i take the absolute value of them.
# exploratory visualization
 during exploratory visualization i have craeted columns to make visualization easier. 
 - i found that users use the bike for along time (1 minute to 24hour) which doesn't make sense ,nobody can ride a bike for whole day
 - most of users are subscriber and this is expected because people use it frequently so it is better for them to be subscriber.
 - It rarely used during night espacially after 12PM .it frequently used from 7AM to 10AM and from 5PM to 8Pm and from 10Am to 5PM it used normally
 - ford bike are used a little bit during weekend but user use it for a long period on weekend
 - users -whatever they are customer or subscriber -use bay wheels service during whole week ,the frequently use it in weekday expect saturday and sunday which is weekend ,so we can say that they use it for work like going to school or going to work
 - the mean duration in minute is 13 minutes with minimum value 1 minutes and maximum value is 1437 minutes(24 hour) ,this doesn't make sense because nobody can ride a bike for whole day ,in my openion the user forget to record the end of his trip,but most of user don't exceed 50 minutes and rare users use it more than an hour
 - they frequently use this service in march ,april,august,september and october ,they use it in december a little bit ,the rest of months ,they used it normally
- people use bikes frequently during weekdays more than that of weekends ,the mean duration of weekends is bigger than that of weekdays,may because during weekday people seeks to go to their distinations queckly,on the other hand on weekend the have free time so no need to be fast.
- as most duration time range from zero to 50 minute i make boxplot visualization in this range to see the relation between subscriber and customer and it seems that the customers concour the subscribers in duration minute as minimum and maximum duration for customers is bigger than that of subscriber and first and third quatile too

- subscriber used bikes more than customer on both weekday and weekend.
- mean of duration of customer is bigger than that of suscriber ,the mean of customer at weekend is bigger that of weekday ,the mean of subscriber is the same during the week if it was at weekend or weekday 
# Key insights
- most of users are subscriber 
- they used it frequently at whole weekday except weekend(saturday and sunday)
- they used it more form 7Am to 8Pm
- most of trip durantion range from 1 minute to 50 minutes.
- they use it in december a little bit








