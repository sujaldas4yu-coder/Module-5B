# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np


arr = np.array([[10, 20, 30],
                [40, 50, 60],
                [70, 80, 90]])


new_col = np.array([100, 200, 300])


arr = np.delete(arr, 1, axis=1)


arr = np.insert(arr, 1, new_col, axis=1)

print("Updated Array:")
print(arr)
```

## Output:
```
Updated Array:
[[ 10 100  30]
 [ 40 200  60]
 [ 70 300  90]]
```

