# MTA Analysis Part 2

This pair is a continuation of MTA Analysis Part 1. Answer the next few problems by building off of the [solutions 
notebook](../mta-pair-1/solution/mta-pair-1-solution.ipynb) for MTA Analysis Part 1.

### Problem 3b
- Work off of the daily maximum `ENTRIES` calculations from Problem 3a. Recall that the `ENTRIES` column contains 
**cumulative entries** on each day. We would now like you to calculate **daily entries**, i.e. the number of new entries gained each day.
- Hint: Group the data by turnstile and use the Pandas `.apply()` method to compute the same differencing function for each turnstile. Check out the `.shift()` and `.diff()` DataFrame methods for this purpose.
- Look through your results. Do they all make sense?

### Problem 4

So far we've been operating on a single turnstile level. Now let's
  combine turnstiles that fall within the same ControlArea/Unit/Station combo. There
  are some ControlArea/Unit/Station groups that have a single
  turnstile, but most have multiple turnstiles -- same value for the
  C/A, UNIT and STATION columns, different values for the SCP column.

We want to combine the numbers together. For each
ControlArea/UNIT/STATION combo, for each day, sum the counts from each
turnstile belonging to that combo. (hint: `pd.groupby`)


#### Problem 5

Similarly, come up with **daily** time series for each STATION, by adding up all the turnstiles in a station.


#### Problem 6

Over multiple weeks, sum total ridership for each station and sort
  them, so you can find out the stations with the highest traffic
  during the time you investigate.

