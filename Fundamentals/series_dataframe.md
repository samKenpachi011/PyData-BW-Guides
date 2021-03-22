# What is Pandas
## Pandas is an open-source library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language. Python with Pandas is used in a wide range of fields including academic and commercial domains including finance, economics, Statistics, analytics. Pandas is built on top on NumPY which is prerequisite to  understanding pandas. [Learn more about NumPy](https://www.tutorialspoint.com/numpy/index.htm)

## Pandas deals with the following three data structures.
  * Series
  * DataFrame
  * Panel

Note-Data Structure:
> A data organization, management and storage format that enables efficient access modification of data values simply put data structure can be used to organize the storage and retrieval of information stored in memory.


What is a Series?:
> A series is a one-dimensional data structure. It can have any data structure like integer, float, and string. It is useful when you want to perform computation or return a one-dimensional array. A series, by definition, cannot have multiple columns.

Try running the code snippets here
  * [Python Shell](https://www.python.org/shell/)
  * [PyNative Code Editor](https://pynative.com/online-python-code-editor-to-execute-python-code/)

```python
import pandas as pd
ds = pd.Series([2, 4, 6, 8, 10])
print(ds)
```

What is a Pandas DataFrame?:
>Pandas DataFrame is a two-dimensional array with labelled data structure having different column types. A DataFrame is a standard way to store data in a tabular format,with rows to store the information and columns to name the information.

```python
import pandas as pd
my_df = pd.DataFrame(data=[4,5,6,7], index=range(0,4), columns=['A'])
print(my_df)
```

What is a Pandas Panel?:
> A panel is a container for three dimensional data. The constructor to the panel looks like -> pandas.Panel(data, items, major_axis, minor_axis, dtype, copy)

  * items − axis 0, each item corresponds to a DataFrame contained inside.
  * major_axis − axis 1, it is the index (rows) of each of the DataFrames.
  * minor_axis − axis 2, it is the columns of each of the DataFrames.

## Execute the following code [here.](https://www.tutorialspoint.com/execute_python_online.php)

```python
#An empty panel
import pandas as pd
emptyPanel = pd.Panel()
print(emptyPanel)
```
```python
# A panel with dimensions
import pandas as pd
import numpy as np
data = np.random.rand(3,4,6)
xPanel = pd.Panel(data)
print(xPanel)
```

## More Resources
  * [PyData Series](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.html)
  * [PyData DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
  * [GeeksforGeeks Pandas Series](https://www.geeksforgeeks.org/creating-a-pandas-series/)
  * [GeeksforGeeks Pandas DataFrame](https://www.geeksforgeeks.org/python-pandas-dataframe/)
 