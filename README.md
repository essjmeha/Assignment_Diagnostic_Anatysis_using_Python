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
