# Numpy Pair Problem

For today's pair, we will use NumPy to complete the following tasks consecutively.

1. Generate three separate 1-dimensional arrays of 10,000 elements each.
* Array 1 should contain numbers randomly drawn from the uniform distribution between 1 and 100
* Array 2 should contain numbers randomly drawn from the normal distribution, with a mean of 0 and a standard deviation of 1
* Array 3 should contain numbers randomly drawn from the binomial distribution, where n=10 and p=0.5

2. For each array, randomly sample 1,000 rows without replacement. (hint: `np.random.choice()`) 

3. For each of the three samples:
* Calculate the mean, median, and standard deviation 
* Find the index and the value of the largest element (hint: `np.argmax()`)
* Find the value of the 75th percentile (hint: `np.percentile()`)

4. Sort each of the three samples in increasing order, then combine them together to create a 1,000 by 3 array. (hint: `np.sort()` and `np.stack()`)  

5. Replace all negative values with 0. Replace all values that exceed 10 with 10.

6. Subtract 5 from all values that exceed 5. (hint: `np.where()`)

7. Produce a fourth column that is the sum of the first two columns. (hint: `np.hstack()`)

8. Use broadcasting to add 1 to each element of the first column, 2 to each element of the second column, 3 to each element of the third column, and 4 to each element of the fourth column.

9. Matrix multiply this 1000x4 array by a 4x1 array of ones. How many unique values are in the resulting product? (hint: `np.unique()`)
