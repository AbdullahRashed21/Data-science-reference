# MTA Analysis Part 1

#### Problem 1   
  
- Open up a new IPython notebook
- Download MTA turnstile data files for the following three dates: ``160903, 160910, 160917```
- Load the files into a pandas DataFrame (hint: `pd.read_csv()` to load files and `pd.concat()` to combine DataFrames)

Your dataframe should look something like this:


|    | C/A   | UNIT   | SCP      | STATION   | LINENAME   | DIVISION   | DATE       | TIME     | DESC    |   ENTRIES |   EXITS                                                                |
|---:|:------|:-------|:---------|:----------|:-----------|:-----------|:-----------|:---------|:--------|----------:|-----------------------------------------------------------------------:|
|  0 | A002  | R051   | 02-00-00 | 59 ST     | NQR456     | BMT        | 08/27/2016 | 00:00:00 | REGULAR |   5799442 |                                                                1966041 |
|  1 | A002  | R051   | 02-00-00 | 59 ST     | NQR456     | BMT        | 08/27/2016 | 04:00:00 | REGULAR |   5799463 |                                                                1966044 |
|  2 | A002  | R051   | 02-00-00 | 59 ST     | NQR456     | BMT        | 08/27/2016 | 08:00:00 | REGULAR |   5799492 |                                                                1966079 |
|  3 | A002  | R051   | 02-00-00 | 59 ST     | NQR456     | BMT        | 08/27/2016 | 12:00:00 | REGULAR |   5799610 |                                                                1966155 |
|  4 | A002  | R051   | 02-00-00 | 59 ST     | NQR456     | BMT        | 08/27/2016 | 16:00:00 | REGULAR |   5799833 |                                                                1966214 |


#### Problem 2

- Let's turn this into a time series.

- Our pandas dataframe has columns called `Date` and `Time` (what datatype did pandas assign to these columns on import?). However, in python and pandas we can convert date and time information to _datetime_ objects, which allow us to do time-based operations

- Using either [pd.to_datetime](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.to_datetime.html) in pandas or the [python datetime library](https://docs.python.org/2/library/datetime.html), combine the `Date` and `Time` columns into a single new column of the datetime datatype

#### Problem 3a

- Each combination of `C/A`, `UNIT`, `SCP`, and `STATION` represents a unique turnstile. Take a look at one specific turnstile on a specific date. What does each row in the dataframe represent?
- Obtain the maximum `ENTRIES` value for each day, for each unique turnstile.