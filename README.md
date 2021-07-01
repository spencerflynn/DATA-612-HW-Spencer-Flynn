# DATA-612-HW1
Data 612 Homework 1 - Spencer Flynn

Showed the .head() and .tail() of the data set, specificying 3 rows. { df.head(3) df.tail(3) }
Printed the column names { df.columns }
Printed to see there are four data types { df.info ---> dtypes: bool(1), float64(6), int64(8), object(6) }
Found the number of rows and columns: (156220, 21) { df.shape }
Found the mean # of prescriptions for each location. { df.groupby('Location')['Number of Prescriptions'].mean() }


# DATA-612-HW2
Data 612 Homework 2 - Spencer Flynn

1.) Imported Libraries and Dataset
2.) Added new column to dataframe that is a converted date column using pd.to_datetime()
3.) Found max of this new column
4.) Found difference in days for all dates from max date
5.) Aftering finding the difference (which is a negative number) I added the two columns to get the date minus the max.
6.) Converted the number of days difference into number of months using np.timedelta64(1, 'M')
7.) Saved the dataset as a csv file using to_csv()

# DATA-612-HW3
Data 612 Homework 3 - Spencer Flynn

1) Imported Libraries and Dataset
2) Used season to generate correlation heatmap, facetgrid plot, and boxplots


# DATA-612-HW4
Data 612 Homework 4 - Spencer Flynn

1) Imported Library and Dataset
2) Concatenated df1 and df2
3) Counted number of nulls values
4) Dropped rows containing null values

# DATA-612-HW5
Data 612 Homework 5 - Spencer Flynn
1) Imported Library and Dataset
2) Changed 'mass' column type from int64 to category using .astype()
3) Changed 'fruit_name' column type from object to string using .astype()

# DATA-612-HW6
Data 612 Homework 6 - Spencer Flynn
1) Imported Librarys and Dataset
2) Created function that uses regex to validate that all 143,375 rows of the date column in my chosen dataset are entered in mm/dd/yyyy format and are real dates.
3) Created dataframe from matrix using pd.DataFrame()
4) Created function to calculate mean, sum, mode, median, and range of my created dataframe and returns results
5) Applied function to dataframe using .apply()

# DATA-612-HW7
Data 612 Homework 7 - Spencer Flynn

MY chosen dataset was the State Drug Utilization Data from 2010.

The metrics I calculated in my summarize_data() function were:
  - average number of prescriptions
  - average total amount reimbursed
  - max total amount reimbursed
  - percentage of number of prescriptions out of the whole dataset

I grouped my data first by Quarter and then by State and applied my function in order to get metrics for each state in each quarter seperately.
In order to view my results better I then sorted the data by descending percent of prescriptions using .sort_values(). In order to keep the states grouped into each quarter I also sorted them by Quarter.
