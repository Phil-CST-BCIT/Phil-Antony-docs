---
layout: default
title: Write Code
nav_order: 5
---

# Writing a basic Python code

<hr>
## Testing Pycharm and Python3
We need to write a simple code to check if Python3 works.

1. Open Pycharm

2. Create a new file, give it any name you like

3. Write the followin code.

4. Save the file, and Press run. <br/>

```python
print("hello world")
```
The output should be as below: <br/>

output: `hello world`.

<hr>

Now, we are good to go!
<hr>

## Writing code
All you need to do is writing the code we have prepared for you.

1. Go to your **_working directory_**.

2. Create a new file, give it a descriptive name for your task

3. import **_pandas_** <br/>

    ```python
    # import pandas means to include the library as a part of your program.
    # pd is just a short name for pandas in your program. You can change it to any name you like.
    import pandas as pd
    ```
4. Define a **_data frame_** for your Excel file.

    ```python
    # df is a short name for data framework.
    # .read_excel() is a program in the libraries you have installed.
    # this line of code read all data in Excel file test, and store the data in df
    df = pd.read_excel('test.xlsx')
    ```
5. Create a new column in the file test.xlsx.

    ```python
    # a new column Test Value is added into test.xlsx file
    df['Test Value'] = df['Units'] * df['UnitCost']
    ```
6. print out the new table.

    ```python
    # prints out the new table, and you can see the column Test Value now is added at the end.
    print(df.head())
    ```
![](https://github.com/Phil-CST-BCIT/Phil-Antony-docs/blob/gh-pages/assets/images/install_pandas.png?raw=true)