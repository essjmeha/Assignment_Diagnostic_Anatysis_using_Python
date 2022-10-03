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
