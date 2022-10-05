# SQL Pair #1

Open up DB Browser for SQLite and open the baby_names database. Remember that you’ll need to navigate to the Execute 
SQL tab, type in a SQL query and run the query by clicking on the triangle button.

## Exercises
Query the baby_names database to answer the following questions:

#### Names Table: Basics

1. Show the top 10 rows from the names table.

  What does each row of data represent in this table?

2. Show only the `name` and `frequency` fields for the first 5 records.

3. Find records for `John`'s born in Washington state after 2010.

  Your output should have 6 records.

4. How many `John`'s are there in the dataset?

  Answer: 2,638,761

5. Show situations where girls were named `John`. In which states and years did this happen the most?

  Answer: Kentucky in 2004

6. What were the top 3 most common female names in New York in the year 2000?
  
  Answer: Emily, Samantha, Ashley


#### Names Table: Aggregations & Operators

7. How many babies are born each year?

  Answer: 3,507,395 in 1951, etc.

8. How many `John`'s were there per state, per year?

  Answer: 100 in Arkansas in 1951, etc.

9. Write a query that tells you how many different female names there were per state, per year.

  Answer: 1,265 in California in 1951, etc.

10. How many records were there in the years 2000, 2001 and 2002?

  Answer: 243,063

11. How many names end with the letter ‘a’ in the table?

  Answer: 7,608



#### Regions Table

12. What are the columns on the region table?

  Answer: state, region

13. How many different regions are there in the region table? (Hint: `DISTINCT`) Can you find the one that looks like a typo?

  Answer: 7