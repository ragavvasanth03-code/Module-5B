# Pandas Program: Create and display a DataFrame with Custom Index Labels

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
data = eval(input())
labels=eval(input())
df = pd.DataFrame(data, index=labels)
print(df)
```

## Output
<img width="1266" height="424" alt="image" src="https://github.com/user-attachments/assets/83604258-586f-44a5-b655-4b7370101d2e" />
<img width="1266" height="438" alt="image" src="https://github.com/user-attachments/assets/7f9059f3-48ce-4397-82c6-3a24dcc5f31c" />
<img width="1261" height="442" alt="image" src="https://github.com/user-attachments/assets/ac1b52d8-d764-4400-9ce3-f77164677e43" />


## Result
Thus, te program has been executed sucessfully 
