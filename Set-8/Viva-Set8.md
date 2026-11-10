# SET 8 – Viva-Voce

### V1. What are vectorized string operations in Pandas? Give one example using `.str`.

Vectorized string operations apply a text function to every value of a column at once, without writing a loop. In Pandas we use the `.str` accessor for this. They are fast, short and automatically skip missing values.

**Example:** `df['Name'].str.upper()` converts every name to capital letters. Other examples are `.str.lower()`, `.str.contains()`, `.str.replace()` and `.str.len()`.

### V2. What is imputation, and why must preprocessing be fitted only on training data when evaluating a model?

Imputation means filling missing values with a sensible estimate such as the mean, median or most frequent value. Imputers and scalers learn numbers (mean, median, standard deviation) from the data.

If they learn from the whole dataset, information from the test data leaks into training, which is called **data leakage** and makes the accuracy look better than it really is.

So we use `fit` (or `fit_transform`) on the training data only, and then only `transform` on the test data.

### V3. What is the difference between a linear SVM kernel and a nonlinear kernel?

A linear kernel separates the classes with a straight line (or a flat plane in higher dimensions), so it works well when the classes can be divided by a straight line.

A nonlinear kernel, such as RBF or polynomial, maps the data to a higher dimension so that a curved boundary can be drawn, which is useful for complex or circular patterns.

Linear is simpler and faster, while RBF is more flexible but can overfit if its parameters are not chosen carefully.