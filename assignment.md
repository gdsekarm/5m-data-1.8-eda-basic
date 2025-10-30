# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you select rows from a DataFrame where any value in the row exceeds a threshold?

```python
import pandas as pd

df = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [10, 20, 30, 40, 50]})
threshold = 30
```

Answer:

```python
filtered_df = df[(df > threshold).any(axis=1)]
print(filtered_df)
```

### Question 2

Question: How do you sort a DataFrame by columns `A` and `B`?

```python
import pandas as pd

df = pd.DataFrame({'A': [2, 1, 2], 'B': [2, 3, 1], 'C': [1, 2, 3]})
```

Answer:

```python
sorted_df = df.sort_values(by=['A', 'B'])
print(sorted_df)

```

### Question 3

Question: How do you concatenate two DataFrames vertically?

```python
import pandas as pd

df1 = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})
df2 = pd.DataFrame({'A': [7, 8, 9], 'B': [10, 11, 12]})
```

Answer:

```python
concatenated_df = pd.concat([df1, df2], )
print(concatenated_df)
```

### Question 4

Question: How do you compute the cumulative sum of a column in a DataFrame?

```python
import pandas as pd

df = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
```

Answer:

```python
df['Cumulative_A'] = df['A'].cumsum()
df
```

### Question 5

Question: How do you convert a Series of strings to uppercase?

```python
import pandas as pd

series = pd.Series(['apple', 'banana', 'cherry'])
```

Answer:

```python
series.str.upper()
```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
