# SET 5 – Viva-Voce

### V1. What is a universal function (ufunc) in NumPy?

A universal function is a NumPy function that works on every element of an array at once, so we do not need to write a loop. Examples are `np.add`, `np.sqrt`, `np.exp` and `np.sin`. For example, `np.sqrt(np.array([4, 9, 16]))` gives `[2. 3. 4.]`. Ufuncs are fast because the work is done in compiled code, and they make programs short and easy to read.

### V2. What is the difference between `duplicated()` and `drop_duplicates()` in Pandas?

`duplicated()` only checks the data: it returns True for each row that is a repeat of an earlier row and False otherwise, and nothing is removed. `drop_duplicates()` actually removes the repeated rows and returns a new DataFrame, keeping the first copy by default. A common way is to count with `df.duplicated().sum()` first and then clean with `df.drop_duplicates()`.

### V3. Why is Logistic Regression suitable for binary classification, and what does the ROC curve show?

Logistic Regression uses the sigmoid function to turn any input into a probability between 0 and 1, and a threshold (usually 0.5) converts it into one of two classes such as pass/fail or buy/not buy. The ROC curve plots the True Positive Rate against the False Positive Rate for all possible thresholds. A curve close to the top-left corner means a good model. The area under the curve (AUC) is 1.0 for a perfect model and 0.5 for random guessing.