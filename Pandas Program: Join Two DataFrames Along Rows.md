# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

student_data1 = {
    'Name': ['Alice', 'Bob'],
    'Age': [20, 21],
    'Course': ['Math', 'Physics']
}

student_data2 = {
    'Name': ['Clarke', 'Diana'],
    'Age': [22, 23],
    'Course': ['Chemistry', 'Biology']
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)

print(combined_df)
```

## Output
```
     Name  Age     Course
0   Alice   20       Math
1     Bob   21    Physics
0  Clarke   22  Chemistry
1   Diana   23    Biology
```
## Result
Thus, the Python program successfully joins two DataFrames row-wise and displays the combined DataFrame.
