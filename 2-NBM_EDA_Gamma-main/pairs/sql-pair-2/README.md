# SQL Pair #2

Open up DB Browser for SQLite and open the baby_names database. Remember that you’ll need to navigate to the Execute 
SQL tab, type in a SQL query and run the query by clicking on the triangle button.

## Exercises
Query the baby_names database to answer the following questions:

1. Which state(s) does not have a region associated with it? Hint: remember DISTINCT

2. What is the most popular boy's name in the South in 2000? Hint: remember GROUP BY

3. What is the third most popular girl’s name in the south in the year 2000?

4. Which state has the largest number of unique names in the year 2000?

5. Which region has the largest number of unique names in the year 2000?

6. Write a query that shows the number of babies born in each region. Exclude the blank region.

  Output
  ```
      region    | num_babies
  ———————+——————
   Mid_Atlantic |   34169982
   Midwest      |   46799608
   Mountain     |   12039060
   New England  |     712977
   New_England  |    9565227
   Pacific      |   33572251
   South        |   73844844
  (7 rows)
  ```


 Extra credit: How could you modify the query to deal with the duplicate region if you only had read access to the database?

  Output
  ```
   region_clean | num_babies
  --------------+------------
   Mid_Atlantic |   34169982
   Midwest      |   46799608
   Mountain     |   12039060
   New_England  |   10278204
   Pacific      |   33572251
   South        |   73844844
  ```

