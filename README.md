# Assignment_Diagnostic_Anatysis_using_Python
How to reduce or eliminate missed appointments on the NHS
questions to answer
Has there been adequate staff and capacity in the networks?
What was the actual utilisation of resources?
What is the number of locations, service settings, context types, national categories, and appointment statuses in the data sets?
What is the date range of the provided data sets, and which service settings reported the most appointments for a specific period?
What is the number of appointments and records per month?
What monthly and seasonal trends are evident, based on the number of appointments for service settings, context types, and national categories?
What are the top trending hashtags (#) on Twitter related to healthcare in the UK?
Were there adequate staff and capacity in the networks?
What was the actual utilisation of resources?
What possible recommendations does the data provide for the NHS?
There are 13,793 records of appointment lengths from 106 regions.  596,821 records of type of appointment from 42 regions.  This DataFrame does not show the location (name or code). For analysis by area I would need to create an additional column providing a location based on the available information in sub location name.  There top five locations to records appointment lengths and categories are inconsistent. The regions (icb_ons_code) E54000057, E54000008, E54000050, E54000048 have the most number of records in all DataFrames.  There are no categories missing within service settings, context types, national categories or appointment statuses.  Appointment_date in incorrect format on ad (object rather than datetime)
Added extra codes to check all columns has data.
Establish the date format for the ad and nc DataFrames using info() and head(). nc was a datetime64, but that the ad was an object.  
Used the dt.strftime to amend the date to d/m/y.
Incorrect dates are being recorded for the min /max  (31/12/21 to 01/01/22).  Further investigation into code is required. 
Created a subset to keep speed up.
By filtering on location ‘NHS North West London ICB - W2U3Z and dates 01/01/22 to 01/06/22, I can see that GP accounted for the most number of records, and 6 unmapped. 
I need to repeat this across the top five locations, and across NHS. 
I need to check the total number of appointments by service setting by location.  The busiest period was Nov 2021 with 30,405,070 and Oct 2021 with 30,303,834.  
Creating a chart would allow me to clearly see a trend.  
I need to look into total number of appointments by location (sum).  
Amended missing value syntax to check all columns with one code.  Deleated unnecessary codes.  
GP appointments accounted for most appointments.  It also had the biggest fluctuations in appointments.   
Care related encounter accounted for most appointments within context tye.  
General Consultation Routine is the most comment type of category.
There is a clear trend throughout the week with number of appointments peaking on Mondays declining Tuesday to Friday, with a big drop on Saturdays and again on Sundays. 
During the Summer month peaks and troughs remain steady and consistent.
Autumn had a gradual increase in appointment when compared to the previous week, until the final week where appointments declined. Could this be do to School Oct half term holidays?
You can see that the 1st of January was a bank holiday.  There was also fewer appointments on 2nd January.  Possibly due to staff being on holiday, or are people more likely to now show up for appointments during holiday periods? 
Easter can also be easily identified during Spring (April).  Again the days surrounding the bank holiday show a comparably lower number of GP appointments. 
Tweets are an opportunity for the NHS to raise awareness about it services, engage with it service users and develop policy and procedures. 
By being aware of the most trending hashtag e.g. #heathcare you increase the likelihood of people interacting with your contents.  
Only 16 tweets (out of 1174) were retweeted at least 200 times.
The proportion of tweeters favouriting a NHS related tweet is low.
1027 (87%) had no response and only 1 was favourited 91 times (8%).
61% of posts hashtags #Healthcare
Further investigation is needed to establish if this also generated the most retweets and favourites.
The initial barplot of words counts showing hashtags words clearly showed the disparity between #healthcare and the remaining words.
Focus on words that appeared at least 20 times (which in this case is top 15 words).
Due to the large variances in values annotating the bars make it easier to the stakeholder to see the frequency of the word.
Rotation of the ticks to 70 degrees.
Added clear headings. 
