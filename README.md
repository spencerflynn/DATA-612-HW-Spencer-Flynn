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
