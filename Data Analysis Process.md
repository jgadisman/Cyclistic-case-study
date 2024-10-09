Import data from Divvy 2019 Q1 and Divvy 2020 Q1

1.  Made columns consistent and merged them into a single dataframe
      - renamed columns to make them consistent with 2020Q1
      - inspected dataframes and look for incongruencies
      - converted ride_id and rideable_type to character so that they can stack correctly
      - stacked individual quarter's data frames into one big data frame
      - removed lat, long, birthyear, and gender fields as this data was dropped beginning in 2020
2.  Cleaned up and added data to prepare for analysis
      - consolidated "members/subscribers" and "casual/customers" from 4 to 2 labels
      - added columns of data (day, month, year) for more opportunities to aggregate the data
      - added a calculated field for length of ride, since the 2020Q1 data did not have a "tripduration" column
      - added "ride_length" to the entire dataframe for consistency
      - remove some rides where tripduration shows up as negative
3.  Conducted descriptive analysis
      - looked at mean, median, max, and min for ride_length and summarize
      - compare casual riders and members using the aggregate function
      - view average ride time each day for members vs casual riders
      - group by user type and week day
      - calculated number of rides and average duration
      - visualized the number of rides by rider type
      - created a visualization for average ride duration
4.  Exported a summary file csv for further analysis
