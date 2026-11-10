# SET 7 – Viva-Voce

### V1. What is the difference between element-wise multiplication and matrix multiplication?

Element-wise multiplication (`a * b`) multiplies the numbers in the same position of two arrays, so both arrays must have the same shape. Matrix multiplication (`a @ b` or `np.dot`) multiplies rows of the first matrix with columns of the second and adds the results; the number of columns of the first must equal the number of rows of the second.

For `[[1,2],[3,4]]` and `[[5,6],[7,8]]`:

- **Element-wise multiplication:** `[[5,12],[21,32]]`
- **Matrix multiplication:** `[[19,22],[43,50]]`

### V2. When is a histogram more useful than a bar plot?

A histogram is used for continuous numerical data. It groups the values into ranges (bins) and shows the shape of the data, such as spread, skewness and outliers. A bar plot is used to compare separate categories, like the average price in each city.

For example, to see how house prices are distributed, we use a histogram of Price, but to compare the average price of City and Suburb, we use a bar plot.

### V3. What assumptions or limitations should be considered when using Linear Regression for prediction?

Linear Regression assumes that the relationship between the inputs and output is a straight line, that the errors (residuals) are random with roughly constant spread, and that the observations are independent. With many inputs, the inputs should not be strongly correlated with each other.

It is sensitive to outliers, cannot capture curved relationships, and gives unreliable predictions outside the range of the training data. Also, a good fit shows a relationship but does not prove cause and effect.