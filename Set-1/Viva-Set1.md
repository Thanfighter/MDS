## SET 1 – Viva-Voce

### V1. What is the difference between a NumPy array and a Python list?

A NumPy array stores elements of the same data type in one block of memory, while a Python list can hold mixed types such as numbers and text. Because of this, arrays are faster and use less memory.

Arrays also allow maths on the whole array at once:

- `np.array([1, 2, 3]) * 2` gives `[2 4 6]`.
- `[1, 2, 3] * 2` just repeats the list.

That is why NumPy is used for data science.

### V2. What does a missing value represent, and when might you use fillna() instead of dropna()?

A missing value (`NaN`) is a cell where the data was not recorded or is unknown.

We use `fillna()` when the dataset is small or every row is valuable, so we replace the gap with the mean, median, or mode instead of losing the row.

We use `dropna()` when only a few rows are affected or a column is almost empty.

**Example:** If Age is missing in 1 of 100 rows, fill it with the mean; if 80% of a column is empty, drop it.

### V3. How does the value of K affect a KNN classifier?

K is the number of neighbours that vote for the class.

- A very small K (like 1) follows every single nearby point, so noise affects it and the model overfits.
- A very large K averages too many points, so the boundary becomes too smooth and the model underfits.
- A medium, odd value (3, 5, 7) usually works best, and odd numbers avoid ties.

We find the best K by comparing accuracy for different K values.