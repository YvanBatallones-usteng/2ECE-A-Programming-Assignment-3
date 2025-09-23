# 2ECEA Programming Assignment - Pandas

This repository contains solutions to programming exercises implemented in Python using Jupyter Notebook. The problems focus on **data manipulation and analysis** using the **Pandas** library.

## Contents

* **Problem 1: Loading and Displaying Data**
  A program that loads the `cars.csv` dataset into a Pandas DataFrame and displays the first five and last five rows of the dataset.

* **Problem 2: Data Analysis with CSV**
  A program that performs further processing on the `cars.csv` dataset, including filtering, grouping, and descriptive statistics using Pandas.

## Files

* `Batallones_Pandas-P1.ipynb` — Jupyter Notebook containing solutions for Problem 1.
* `Batallones_Pandas-P2.ipynb` — Jupyter Notebook containing solutions for Problem 2.
* `cars.csv` — CSV dataset used for data manipulation and analysis.

## Example Usage

### Problem 1

**Code:**

```python
import pandas as pd

# Load the dataset into a DataFrame
cars = pd.read_csv("cars.csv")

# Display the first five rows
print("First 5 rows:")
print(cars.head())

# Display the last five rows
print("\nLast 5 rows:")
print(cars.tail())
```
This program reads the `cars.csv` dataset into a Pandas DataFrame called `cars`. The `.head()` method shows the first five rows, while `.tail()` shows the last five rows, giving a quick overview of the dataset’s structure and contents.

**Sample Output (shortened):**

```
First 5 rows:
            Model   mpg  cyl   disp   hp  ...
0       Mazda RX4  21.0    6  160.0  110  ...
1   Mazda RX4 Wag  21.0    6  160.0  110  ...
...

Last 5 rows:
           Model   mpg  cyl   disp   hp  ...
27  Lotus Europa  30.4    4   95.1  113  ...
28  Ford Pantera  15.8    8  351.0  264  ...
...
```

### Problem 2

**Code:**

```python
import pandas as pd

# Load the dataset
df = pd.read_csv("cars.csv")

# Filter and display the row where Model = 'Mazda RX4'
print(df[df['Model'] == 'Mazda RX4'])
```
Here, the dataset is loaded again into a DataFrame. A filter is applied to the `Model` column using a boolean condition, and only the row where the model is `"Mazda RX4"` is displayed. This shows how Pandas can be used to quickly locate specific entries in a dataset.

**Sample Output:**

```
       Model   mpg  cyl   disp   hp  drat    wt   qsec  vs  am  gear  carb
0  Mazda RX4  21.0    6  160.0  110  3.90  2.62  16.46   0   1     4     4
```

---

## Author / Student Info

* **Name:** Yvan Reyan M. Batallones
* **Course:** 2ECE-A
* **Activity:** Programming Assignment 3 - Pandas

---
