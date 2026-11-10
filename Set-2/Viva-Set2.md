## SET 2 – Viva-Voce

### V1. What is the purpose of ranking or sorting values in Pandas?

Sorting arranges rows from smallest to largest (or the reverse), so we can quickly see top or bottom values.

Ranking gives each value a position number, such as 1 for the highest, without changing the order of rows; equal values get the average rank.

Both are useful for questions like "who are the top 5 students" or "which product sells the most".

In Pandas, we use:
- `sort_values()`
- `rank()`

### V2. What is Min-Max scaling, and what range does it usually produce?

Min-Max scaling rescales a column using:

`(x - min) / (max - min)`

It usually produces values between 0 and 1:
- The smallest value becomes 0.
- The largest value becomes 1.

We use it when features have different units, like age and salary, so that large numbers do not dominate the model.

Its weakness is that one big outlier can squeeze all other values close to 0.

### V3. What is a decision boundary in SVM, and what is the role of the support vectors?

A decision boundary is the line (or surface) that separates one class from another; points on one side get class A and the other side class B.

A linear SVM chooses the line that leaves the widest gap (margin) between the two classes.

**Support vectors** are the data points closest to this line.

They alone decide where the line sits:
- If we remove other points, nothing changes.
- If we move a support vector, the line shifts.