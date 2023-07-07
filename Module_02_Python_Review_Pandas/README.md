# Pandas

## Topics covered in today's module

* Introduction to Pandas
* Tabular Data
* Operations on Tabular data

## Main takeaways from doing today's assignment
- You can create dataframes via dictionaries, or by organizing indices, rows and columns by lists
- You can access general info. on column names, number of objects in each column and datatype by df.info()
- you enumerate through lists via enumerate(lists):
- You can reset indices via reset_index(drop=True)
- The nunique() prints the number of unique classes or values in a column
- you can make a boolean mask via df[df['Class'] == value]]
- there is a built in function to get the index for the min. value of a column called idxmin()
- .iloc, .loc, .iat, .at are all methods to index through a dataframe
- you can set pd display options via pd.set_option()
- you can't chain together operators in a statement like 100<df.index<121
- df.sort_values() and df.sort_index() filter by column or index and can be ordered ascendingly or descendingly

## Challenging, interesting, or exciting aspects of today's assignment
I had some trouble with answer 5, specifically figuring out what the right order of sorting values and sorting indices was. Originally, I though I had to write more than one line of code but I learned that I can actually combine multiple methods into one, which was convenient.

## Additional resources used 
Unique values in pd column: https://stackoverflow.com/questions/32072076/find-the-unique-values-in-a-column-and-then-sort-them

Python operators syntax: https://www.w3schools.com/python/python_operators.asp

Excluding rows when slicing pd.df: https://stackoverflow.com/questions/65378869/how-to-drop-rows-by-slice

Dropping pandas column: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.drop.html

Sorting by ascending order: https://stackoverflow.com/questions/37787698/how-to-sort-pandas-dataframe-from-one-column

Syntax correction and general code debugging: ChatGPT
