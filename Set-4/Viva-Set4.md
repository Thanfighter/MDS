## SET 4 – Viva-Voce

### V1. What are Q1, Q3, and IQR?

- **Q1 (First Quartile):** The 25th percentile; 25% of the data is below it.
- **Q3 (Third Quartile):** The 75th percentile; 75% of the data is below it.
- **IQR (Interquartile Range):** Shows the spread of the middle 50% of the data.

**Formula:**

`IQR = Q3 - Q1`

Values below `Q1 - 1.5 * IQR` or above `Q3 + 1.5 * IQR` are treated as outliers.

**Example:**

If Q1 = 31250 and Q3 = 35750:

- IQR = 4500
- Upper limit = 42500

### V2. Does correlation prove that one variable causes another? Explain briefly.

No. Correlation only tells how strongly two variables move together, from −1 to +1, but not why.

**Example:** Ice-cream sales and drowning cases both rise in summer, yet ice-cream does not cause drowning; a hidden third factor, hot weather, affects both.

To prove cause and effect, we need controlled experiments or strong domain knowledge, not just a correlation value.

### V3. What is a residual in regression, and what pattern would you hope to see in a residual plot?

A residual is the difference between the actual value and the predicted value.

**Formula:**

`residual = actual - predicted`

In a residual plot, we hope to see points scattered randomly around the zero line, with no curve or funnel shape.

This means the model captured the pattern and the errors are only random noise.

- **Curve:** Means the relationship is not linear.
- **Funnel shape:** Means the error size changes with the prediction.