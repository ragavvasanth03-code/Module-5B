# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
~~~
import numpy as np
d=eval(input())
arr=np.array(d)
print("Given array")
print(f" {arr}")

print(f"\n{np.sort(arr,axis=0)}")
~~~

## Output
![WhatsApp Image 2025-10-20 at 15 53 28_ccbaac98](https://github.com/user-attachments/assets/6c108513-51b9-4fbe-8ea1-3f3561128532)

## Result
Thus , the program has been executed succesfully.

# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
~~~
import numpy as np
x = np.array([10, 4, 6, 8, 5])
y = np.array([7, 4, 9, 3, 5])
greater = x > y     
equal = x == y       
indices = np.where(x >= y)
print("x:", x)
print("y:", y)
print("x > y:", greater)
print("x == y:", equal)
print("Indices where x >= y:", indices)
print("Values of x where x >= y:", x[indices])

~~~

## Output
<img width="530" height="240" alt="Screenshot 2025-10-20 184845" src="https://github.com/user-attachments/assets/ea210369-fa4a-4d11-b526-1fd5e4cc97e4" />

## Result
Thus , the program has been executed succesfully.

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
~~~
import numpy as np
arr = np.array( [[1,2,3],[4,5,6],[7,8,9]])
new_col = np.array([10,11,12])
arr_deleted = np.delete(arr, 1, axis=1)
updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)
print("Updated Array:\n", updated_arr)

~~~

## Output
<img width="344" height="176" alt="Screenshot 2025-10-20 185545" src="https://github.com/user-attachments/assets/d1a00c7d-1bd9-41b6-b148-5500e7a3e2ab" />

## Result
Thus , the program has been executed succesfully.

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
~~~
import pandas as pd
import numpy as np
data = eval(input())
labels=eval(input())
df = pd.DataFrame(data, index=labels)
print(df)
~~~

## Output



<img width="1130" height="389" alt="Screenshot 2025-10-20 185900" src="https://github.com/user-attachments/assets/41e9ded3-f6c4-4aa2-9513-64794751ee6a" /><img width="1134" height="394" alt="Screenshot 2025-10-20 185918" src="https://github.com/user-attachments/assets/41d530e0-4f74-4eca-8be2-a0990e5294d1" /><img width="1134" height="398" alt="Screenshot 2025-10-20 185933" src="https://github.com/user-attachments/assets/86d212be-00a1-4b24-a663-0367009ec8a9" />



## Result
Thus , the program has been executed succesfully.

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
~~~
import pandas as pd
dict1 = eval(input())
dict2 = eval(input())
df1 = pd.DataFrame(dict1)
df2 = pd.DataFrame(dict2)
print("Original DataFrames:")
print(df1)
print("-------------------------------------")
print(df2)
joined_df = pd.concat([df1, df2], axis=0)

print("\nJoin the said two dataframes along rows:")
print(joined_df)
~~~

## Output
<img width="1119" height="676" alt="Screenshot 2025-10-20 154259" src="https://github.com/user-attachments/assets/c6a75b2d-26b5-4301-b9e1-b3cc6f33c907" /><img width="813" height="773" alt="Screenshot 2025-10-20 154622" src="https://github.com/user-attachments/assets/d1988b1a-4a7b-4fa1-9699-75457201d28d" />


## Result
Thus , the program has been executed succesfully.


