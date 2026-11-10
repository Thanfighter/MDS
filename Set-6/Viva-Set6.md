# SET 6 – Viva-Voce

### V1. What is one difference between `apply()` and `map()` in Pandas?

`map()` works only on a single column (Series) and is mostly used to replace values using a dictionary or a simple function, like `df['Gender'].map({'M': 'Male', 'F': 'Female'})`. `apply()` is more flexible: it can run any function on a Series, and it can also work on rows or columns of a whole DataFrame. For example, `df['Marks'].apply(np.sqrt)` applies the square root to every mark.

### V2. What is standardization, and how does it differ from Min-Max scaling?

Standardization (z-score scaling) changes each value to `(x - mean) / std`, so the column gets mean 0 and standard deviation 1. The values can be negative and are not limited to a fixed range. Min-Max scaling instead squeezes all values into 0 to 1 using the minimum and maximum. Standardization is usually better when the data has outliers or is roughly bell-shaped, and Min-Max is used when we need a fixed range.

### V3. Why should numerical features often be scaled before applying KNN?

KNN decides using the distance between points, so a feature with large numbers dominates the distance. For example, a salary difference of 5000 completely hides an age difference of 5, even if age is equally important. Scaling brings all features to a similar range so that each one contributes fairly to the distance. This usually improves the accuracy of KNN.