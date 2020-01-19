# Explore-U.S.-Births
Practice the basics of Python by analyzing births in the U.S.
1. Introduction To The Dataset
  Read the CSV file "US_births_1994-2003_CDC_NCHS.csv" into a string.
  Split the string on the newline character ("\n").
2. Converting Data Into A List Of Lists
  Create a function named read_csv()
  Use the read_csv() function to read in the file "US_births_1994-2003_CDC_NCHS.csv" and assign the result to cdc_list.
3. Calculating Number Of Births Each Month
  Create a function named month_births() 
  Use the month_births() function to calculate the monthly totals for the dataset and assign the result to cdc_month_births. Display the dictionary.
4. Calculating Number Of Births Each Day Of Week
  Create a function named dow_births() that takes a single, required argument (a list of lists) and returns a dictionary containing the total number of births for each unique value of the day_of_week column.
  Use the dow_births() function to return the day-of-week totals for the dataset and assign the result to cdc_day_births. Display the dictionary.
5. Creating A More General Function
  Create a function named calc_counts()
  Use the calc_counts() function to:
    Return the yearly totals for the dataset and assign the result to cdc_year_births.
    Return the monthly totals for the dataset and assign the result to cdc_month_births.
    Return the day-of-month totals for the dataset and assign the result to cdc_dom_births.
    Return the day-of-week totals for the dataset and assign the result to cdc_dow_births.
