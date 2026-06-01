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
# Pandas Program: Join Two DataFrames Along Rows

import pandas as pd

# First DataFrame
student_data1 = {
    'student_id': [1, 2, 3],
    'name': ['Alex', 'Amy', 'Allen'],
    'marks': [85, 90, 78]
}

# Second DataFrame
student_data2 = {
    'student_id': [4, 5, 6],
    'name': ['John', 'Sara', 'David'],
    'marks': [88, 92, 80]
}

# Create DataFrames
df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

# Concatenate DataFrames row-wise
new_df = pd.concat([df1, df2], axis=0)

# Display result
print(new_df)
```

## Output:
```
   student_id   name  marks
0           1   Alex     85
1           2    Amy     90
2           3  Allen     78
0           4   John     88
1           5   Sara     92
2           6  David     80
```
