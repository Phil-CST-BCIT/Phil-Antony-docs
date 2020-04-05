---
layout: default
title: Download Libraries
nav_order: 4
has_toc: true
---

# Download Libaries

<hr>
A Python library is a set of programs written by experienced programmers. The library provides some predefined functionalities and lets you focus on your task without thinking of how to write code to build those functionalities. In other words, a library is some code you can instantly use in your program.

We need to download three libraries for our project, and they are
- [pandas](https://phil-cst-bcit.github.io/Phil-Antony-docs/docs/glossary/)
- [xlrd](https://phil-cst-bcit.github.io/Phil-Antony-docs/docs/glossary/)
- [openpyxl](https://phil-cst-bcit.github.io/Phil-Antony-docs/docs/glossary/)
<hr>

First of all, check if you have installed **_Python 3_**

![](./assets/images/note.png)

1. Open a terminal
    1. Click launchpad
    2. Click Other
    3. Click Terminal
![](./assets/images/launchpad.png)

2. Change directory to your working directory
`cd /absolute_path_to/your_working_directory/`

3. Type the following command in your terminal
`which python3`
  * If you have the following line, it means you have **_Python 3_** on your computer.
`/usr/local/bin/python3`
  * If it tells you
`Python3 not found:`
    It means you don't have **_Python 3_** installed on your computer.
    Click [here](https://phil-cst-bcit.github.io/Phil-Antony-docs/docs/install/) to step 1 to install **_Python 3_**.

4. We'll use a program **_PIP3_** to install libraries. **_PIP3_** is a  installer bundled with **_Python3_**.

5. Install Pandas. Type in the following command in terminal
`pip3 install pandas`
![](./assets/images/install_pandas.png)

When you see the message above in the terminal, you have Pandas installed.There is chance the installation might fail, please check [Troubleshooting](https://phil-cst-bcit.github.io/Phil-Antony-docs/docs/troubleshooting/) for solutions.

6. Install xlrd.
`pip3 install xlrd`

7. Install openpyxl
`pip3 install openpyxl`

The prompt messages in the terminal after success installation are similar to the one in Pandas.