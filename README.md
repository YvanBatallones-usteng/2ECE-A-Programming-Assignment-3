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

**Problem 1 Input:**

```python
import pandas as pd

# Load the dataset into a DataFrame
cars = pd.read_csv("cars.csv")

# Display the first five and last five rows
print("First 5 rows:")
print(cars.head())

print("\nLast 5 rows:")
print(cars.tail())
````

**Sample Output:**

```text
First 5 rows:
                 Model   mpg  cyl   disp   hp  drat     wt   qsec  vs  am  gear  carb
0            Mazda RX4  21.0    6  160.0  110  3.90  2.620  16.46   0   1     4     4
1        Mazda RX4 Wag  21.0    6  160.0  110  3.90  2.875  17.02   0   1     4     4
2           Datsun 710  22.8    4  108.0   93  3.85  2.320  18.61   1   1     4     1
3       Hornet 4 Drive  21.4    6  258.0  110  3.08  3.215  19.44   1   0     3     1
4    Hornet Sportabout  18.7    8  360.0  175  3.15  3.440  17.02   0   0     3     2


Last 5 rows:
              Model   mpg  cyl   disp   hp  drat     wt   qsec  vs  am  gear  carb
27     Lotus Europa  30.4    4   95.1  113  3.77  1.513  16.90   1   1     5     2
28   Ford Pantera L  15.8    8  351.0  264  4.22  3.170  14.50   0   1     5     4
29     Ferrari Dino  19.7    6  145.0  175  3.62  2.770  15.50   0   1     5     6
30    Maserati Bora  15.0    8  301.0  335  3.54  3.570  14.60   0   1     5     8
31      Volvo 142E   21.4    4  121.0  109  4.11  2.780  18.60   1   1     4     2
```

**Problem 2 Input:**

```python
import pandas as pd

# Load the dataset
df = pd.read_csv("cars.csv")

# Display the row that contains the ‘Model’ of ‘Mazda RX4’
df[df['Model'] == 'Mazda RX4']
```

**Sample Output:**

```text
       Model   mpg  cyl   disp   hp  drat    wt   qsec  vs  am  gear  carb
0  Mazda RX4  21.0    6  160.0  110  3.90  2.62  16.46   0   1     4     4
```

## Author / Student Info

* **Name:** Yvan Reyan M. Batallones
* **Course:** 2ECE-A
* **Activity:** Programming Assignment 3- Pandas

```
