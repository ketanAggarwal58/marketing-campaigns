# Pandas - Python Library

This document holds the information related to Pandas library of Python.

*Source* - https://www.w3schools.com/python/pandas/default.asp

## Introduction

Pandas is a python library which is used to analyze, cleaning, exploration and manipulation of data.

Pandas was created by **Wes Mckinney** and name pandas has a reference to **Panel Data** and **Python Data Analysis**

Pandas has three (3) different section which are listed as follows:

1. Analysis
2. Cleaning Data
3. Corelation & Plotting

To use pandas, we need to first import pandas into our python codebase.

```
import pandas as pd
```

## Analysis

Inside pandas, we have multiple functions which can be used to analyse the data using python.

### Pandas class Series and constructors

#### _Introduction_

A pandas series is like a column in a table which holds multiple data types, It is a one-dimensional array holding data of any sort.

```
import pandas as pd

a = [1, 7, 2]

myData = pd.Series(a)

print(myData)
```

This **series class** has a special capability that helps us label data in the dataset. By default, values in the dataset are labelled with the index values which starts from `0`.


```
print(myData[0])
```

#### _Create Lables_


The series class allows you to create your own labels.

```
myvar = pd.Series(a, index = ["x", "y", "z"])
```

The following way represents how we can reference our labels. 

```
print(myvar["x"])
```



#### _Key/Value Objects_

We can also access the **Key/values objects** using the Series Class.

```
calories = {"day1": 420, "day2": 380, "day3": 390}

myvar = pd.Series(calories)

print(myvar)
```

We can also select a few items of the **Key/Value Object**

```
calories = {"day1": 420, "day2": 380, "day3": 390}

myvar = pd.Series(calories, index= ["day1", "day2"])

print(myvar)
```

### Pandas Dataframe Class

A Pandas Dataframe is a 2 Dimensional data structure, like a 2 Dimensional Array, or a table with rows and columns.

```
import pandas as pd

data = {
  "calories": [420, 380, 390],
  "duration": [50, 40, 45]
}

df = pd.DataFrame(data)

print(df) 
```

#### Locate Row Function

The data frame class has many functions, but this function is unique as it helps to identify a row in the data frame. 

To use the functionality you need to use the `loc` attribute in the data frame

```
print(df.loc[0])
```

you can also pass a list in the `loc` attribute.

```
print(df.loc[[1,2]])
```

