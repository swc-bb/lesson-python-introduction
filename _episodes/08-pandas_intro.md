---
title: "Introduction to pandas"
teaching: 20
exercises: 15
questions:
- "What is pandas?"
- "How to use the pandas API?"
objectives:
- "Learn how to use pandas for exploring and analyzing spreadsheet like data sets."
keypoints:
- "Pandas rulez!"
---

## The `pandas` library


The `pandas` library was created by Wes Mckinney in 2011. `pandas` provides **data structures** and **functions** for manipulating, 
processing, cleaning and crunching data. In the Python ecosystem `pandas` is the state-of-the-art tool for tabular or spreadsheet-like data
 in which each column may be a different type (`string`, `numeric`, `date`, or otherwise). It provides sophisticated indexing functionality 
 to make it easy to reshape, slice and dice, perform aggregations, and select subsets of data. 
 
`pandas` relies on other packages, such as `NumPy`, short for Numerical Python, one of the foundational package for scientific computing
in Python and `SciPy`, a collection of packages addressing a number of different standard problem domains in scientific computing. 
Further `pandas` integrates `matplotlib`, probable the most popular Python library for plotting and 2D data visualizations. 


Once installed (for details refer to the [online documentation](https://pandas.pydata.org/pandas-docs/stable/install.html)),
we import the `pandas` library into our Python session by using the canonical alias `pd`.

~~~
import pandas as pd
~~~
{: .language-python}

The pandas library has two workhorse data structures: _Series_ and _DataFrame_.

***

### `pd.Series` object 

A Series is a one-dimensional array-like object containing an array of data and an associated array of data labels, called its _index_. We may
create a `pd.Series` object by calling the `pd.Series()` function. 


> ## Functions and their arguments
>
> To get help on a function, its general usage, its input arguments and its return values us the `?` or `??` magic.    
>
> ~~~
> ?pd.Series
> # or
> ??pd.Series
> ~~~
>
> A pop-up window appears with many useful information on the particular function call.
> {: .language-python}
{: .callout}


The documentation returns the following strcuture of the function call

~~~
pd.Series(data=None, index=None, dtype=None, name=None, copy=False, fastpath=False)
~~~ 
{: .output}



~~~
from numpy import random
random.seed(123) # set seed for reproducibility
my_data = random.randint(low=-10, high=10, size=26,)
my_data
~~~
{: .language-python}

~~~
array([  3,  -8,  -8,  -4,   7,   9,   0,  -9, -10,   7,   5,  -1, -10,
         4, -10,   5,   9,   4,  -6, -10,   6,  -6,   7,  -7,  -8,  -3])
~~~
{: .output}


~~~
# create a pd.Series object
s = pd.Series(data=my_data, name="my_pandas_series")
s
~~~
{: .language-python}

~~~
0      3
1     -8
2     -8
3     -4
4      7
5      9
6      0
7     -9
8    -10
9      7
10     5
11    -1
12   -10
13     4
14   -10
15     5
16     9
17     4
18    -6
19   -10
20     6
21    -6
22     7
23    -7
24    -8
25    -3
Name: my_pandas_series, dtype: int32])
~~~
{: .output}


**Element-wise arithmetic**

***
### `pd.Series` attributes

***

#### Selection and slicing by index

***
### `pd.Series` methods

***

### `pd.DataFrame` object



The primary object in pandas that will be used in this book is the DataFrame, a twodimensional
tabular, column-oriented data structure with both row and column labels:

***

### `pd.DataFrame` attributes

***

#### Selection and slicing by indices

**The column index**

**The row index**

**Row and columns indices**

***
#### Manipulating columns, rows and particular entries

**Add a row to the data set**

**Add a column to the data set**

**Change a particular entry**

***

### `pd.DataFrame` methods


*** 

**`groupby` method**

Split-apply-combine paradigm

**`plot` method**

***