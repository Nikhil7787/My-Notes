# Pandas



### functions in pandas for data manipulation and analysis: </br>

1.	Data Input/Output: </br>
•	read_csv(): Read a CSV file into a DataFrame. </br>
•	read_excel(): Read an Excel file into a DataFrame. </br>
•	read_sql(): Read from a SQL database into a DataFrame. </br>
•	to_csv(): Write a DataFrame to a CSV file. </br>
•	to_excel(): Write a DataFrame to an Excel file. </br>
•	to_sql(): Write a DataFrame to a SQL database. </br>
2.	Data Exploration: </br>
•	head(): View the first few rows of a DataFrame. </br>
•	tail(): View the last few rows of a DataFrame. </br>
•	info(): View a concise summary of a DataFrame. </br>
•	describe(): Generate descriptive statistics of a DataFrame. </br>
•	shape: Get the dimensions of a DataFrame (rows, columns). </br>
3.	Data Selection/Manipulation: </br>
•	loc[]: Access a group of rows and columns by label(s). </br>
•	iloc[]: Access a group of rows and columns by integer position(s). </br>
•	at[]: Access a single value for a row/column label pair. </br>
•	iat[]: Access a single value for a row/column pair by integer position. </br>
•	drop(): Drop specified rows or columns from a DataFrame. </br>
•	fillna(): Fill missing values in a DataFrame. </br>
•	replace(): Replace values in a DataFrame. </br>
4.	Data Aggregation/Grouping: </br>
•	groupby(): Group DataFrame using a mapper or by a Series of columns. </br>
•	agg(): Aggregate using one or more operations over specified axis. </br>
•	pivot_table(): Create a spreadsheet-style pivot table as a DataFrame. </br>
5.	Data Cleaning/Preprocessing: </br>
•	drop_duplicates(): Remove duplicate rows from a DataFrame. </br>
•	astype(): Cast a pandas object to a specified dtype. </br>
•	rename(): Rename columns or index in a DataFrame. </br>
•	sort_values(): Sort DataFrame by one or more columns. </br>
6.	Data Visualization: </br>
•	plot(): Plot data. </br>
•	hist(): Draw histogram of DataFrame's columns. </br>
•	boxplot(): Make a box plot of the DataFrame columns. </br>
•	scatter(): Make a scatter plot of two columns. </br>
7.	Data Concatenation/Merging: </br>
•	concat(): Concatenate pandas objects along a particular axis. </br>
•	merge(): Merge DataFrame or named Series objects with a database-style join. </br>
8.	Data Reshaping: </br>
•	melt(): Unpivot a DataFrame from wide format to long format. </br>
•	pivot(): Return reshaped DataFrame organized by given index / column values. </br>
•	stack(): Stack the prescribed level(s) from columns to index. 

<be>
<br>
<br>

### Here are some attributes of a DataFrame object in pandas:

1.	**index**: The row labels of the DataFrame. </br>
2.	**columns**: The column labels of the DataFrame. </br>
3.	**dtypes**: The data types of each column in the DataFrame. </br>
4.	**shape**: The dimensions of the DataFrame (number of rows, number of columns). </br>
5.	**size**: The total number of elements in the DataFrame. </br>
6.	**values**: The data stored in the DataFrame as a 2D NumPy array. </br> 
7.	**empty**: A boolean indicating whether the DataFrame is empty or not. </br>
8.	**ndim**: The number of dimensions (axes) of the DataFrame. </br>
9.	**axes**: A list of the row and column axes labels. </br>
10.	**name**: The name of the DataFrame. </br>
11.	**loc**: Access a group of rows and columns by label(s). </br>
12.	**iloc**: Access a group of rows and columns by integer position(s). </br>
13.	**iat**: Access a single value for a row/column pair by integer position. </br>
14.	**at**: Access a single value for a row/column label pair. </br>
15.	**style**: Access style-related properties for the DataFrame. </br>
16.	**columns.name**: The name of the columns. </br>
17.	**index.name**: The name of the index.


<br>
These are some of the most commonly used attributes of a DataFrame object in pandas. Depending on the version of pandas and your specific needs, there may be additional attributes available. You can access these attributes by using dot notation (e.g., df.index, df.columns, etc.).
