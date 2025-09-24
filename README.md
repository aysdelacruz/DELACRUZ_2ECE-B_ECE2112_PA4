# DELACRUZ_2ECE-B_ECE2112_PA4

## PROBLEM 1 – DATA CLEANING

For the first problem, I started by loading up pandas since that’s what we usually use for handling data. I read the Excel file into a
DataFrame so I could actually work with the rows and columns. The first thing I did was take a quick look at the data using .head() just to
see what it looked like. Some of the column names were kind of long and hard to type, so I renamed them into shorter versions like “ID” or
“Grade” to make things easier while coding. After that, I checked if there were any missing values using .isnull().sum() and then removed
rows that had blanks using .dropna(). I also checked if there were duplicate rows, since that would mess up the results, and dropped them
with .drop_duplicates(). Another thing I looked at was the data types of each column with .dtypes. Some columns weren’t in the right
format, so I made sure the numeric values were actually treated as numbers (int or float). Once everything looked clean, I saved the new
dataset as cleaned_data.csv so I could use it later for the next steps.

## PROBLEM 2 – VISUALIZATION

For the second problem, it was more about making sense of the data by plotting graphs. I used Matplotlib and Seaborn to make bar charts
that show the averages. The first graph I made compared the average scores for each track. I set “Track” on the x-axis and “Average” on
the y-axis, and then made a bar plot that shows the mean scores for Instrumentation, Communication, and Microelectronics. I added a title
and labels so it was clear what the chart was showing. Next, I wanted to see if gender had any difference in the averages. I did the same
thing but this time with “Gender” on the x-axis. The bar chart showed the average for male and female students side by side.
Finally, I did one more comparison based on hometown. I set the x-axis to “Hometown” and plotted the averages for students from Luzon,
Visayas, and Mindanao. Again, I added titles and labels to keep the chart easy to read.
