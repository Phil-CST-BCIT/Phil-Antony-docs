---
layout: default
title: Write Code
nav_order: 5
---

# Writing code

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

## Get the columns you want and generate a new file.
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
    print(df.head())
    ```
    ![](https://github.com/Phil-CST-BCIT/Phil-Antony-docs/blob/gh-pages/assets/images/origin_table.png?raw=true)

5. Create a new column in the file test.xlsx.

    ```python
    # a new column Test Value append at the end of the table.
    df['new_column'] = df['the_column_you_are_interested']
    ```
6. print out the new table.

    ```python
    # prints out the new table and check if everything ok
    print(df.head())
    ```
    ![](https://github.com/Phil-CST-BCIT/Phil-Antony-docs/blob/gh-pages/assets/images/new_table.png?raw=true)

7. create a copy of the original table and save it.

    ```python
    # give your new Excel file a name, here it is new_table.xlsx
    writer = pd.ExcelWriter('new_table.xlsx')
    # give the new sheet a name
    df.to_excel(writer, 'new_sheet')
    # don't forget to save your file
    writer.save()
    ```

    ![](https://github.com/Phil-CST-BCIT/Phil-Antony-docs/blob/gh-pages/assets/images/file_created.png?raw=true)

The entire code

    ```python
    import pandas as pd

    df = pd.read_excel('test.xlsx')
    df['new_c1'] = df['Units']
    df['new_c2'] = df['UnitCost']
    df['new_c3'] = df['Total']
    writer = pd.ExcelWriter('new_table.xlsx')
    df.to_excel(writer, 'new_sheet')
    print(df.head())
    writer.save()
    ```

Now you have the new table, you can just hide all the unneccssary columns and send your boss the new file.
Job done!