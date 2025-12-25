# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Alice', 'Bob', 'Clarke', 'Diana'],
    'score': [85, 92, 78, 90],
    'attempts': [1, 2, 3, 1],
    'qualify': ['yes', 'yes', 'no', 'yes']
}

labels = ['a', 'b', 'c', 'd']

df = pd.DataFrame(exam_data, index=labels)

print(df)
```

## Output
```
     name  score  attempts qualify
a   Alice     85         1     yes
b     Bob     92         2     yes
c   Clarke     78         3      no
d   Diana     90         1     yes
```
## Result
Thus, the Python program successfully creates a Pandas DataFrame from the given dictionary with custom index labels and displays it.
