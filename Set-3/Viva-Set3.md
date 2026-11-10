## SET 3 – Viva-Voce

### V1. What is the difference between indexing and slicing in NumPy?

Indexing picks a single element using its position, for example `a[2]` gives the third element because counting starts from 0.

Slicing picks a range of elements, for example `a[1:4]`, and returns a smaller array; the end position is not included.

- Negative index like `a[-1]` counts from the end.
- In a 2D array:
  - `b[1, 2]` is indexing (one value).
  - `b[:2, 1:]` is slicing (a block of values).

### V2. What is label encoding, and when can it be unsuitable for nominal categories?

Label encoding converts text categories into numbers, such as Female = 0 and Male = 1.

It is fine for:
- Ordered (ordinal) data like Low < Medium < High.
- Target labels.

It is unsuitable for nominal categories, which have no order, because the model may think that a bigger number means something more.

**Example:** Chennai = 0, Hyderabad = 1, Mumbai = 2 wrongly suggests Mumbai is "greater" than Chennai, so one-hot encoding (`pd.get_dummies`) is better.

### V3. What does Gini impurity measure, and how does a Decision Tree use it to choose a split?

Gini impurity measures how mixed the classes are inside a node.

- It is 0 when all samples belong to one class (pure).
- It becomes larger when classes are mixed (maximum 0.5 for two classes).

**Formula:**

`1 - sum(p²)`

The tree tries possible splits, calculates the Gini of the two child nodes, and chooses the split that reduces impurity the most.

It repeats this on each child until the nodes are pure or the maximum depth is reached.