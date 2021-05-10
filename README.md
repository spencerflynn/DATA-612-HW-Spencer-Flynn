# DATA-612-HW1
Data 612 Homework 1 - Spencer Flynn

Showed the .head() and .tail() of the data set, specificying 3 rows. { df.head(3) df.tail(3) }
Printed the column names { df.columns }
Printed to see there are four data types { df.info ---> dtypes: bool(1), float64(6), int64(8), object(6) }
Found the number of rows and columns: (156220, 21) { df.shape }
Found the mean # of prescriptions for each location. { df.groupby('Location')['Number of Prescriptions'].mean() }
