### The Actual Logic Code.py  Holds the actual code of the project Main.py and App.py were built with the help of AI


Expense Tracker

A simple personal expense tracker, originally written as a console (terminal-based) Python program and later turned into an interactive Streamlit web app.

Files in this project
Main.py — Holds the core logic only: reading expenses from the txt file, writing/appending new expenses, rewriting the file when one is deleted, and calculating totals/category totals. No Streamlit code lives here — it can be understood and tested on its own.
app.py — The Streamlit web app. This is the file you actually run. It imports the functions from Main.py and builds the interactive UI around them (sidebar menu, forms, tables, charts, color theme).
expenses.txt — The actual data file where every expense is stored, one per line, in the format date|category|description|amount. This file is created automatically the first time you add an expense — you don't need to create it yourself. Deleting this file will erase your expense history.
README.md — This file. Explains what everything does.
How to run it
Make sure Main.py, app.py, and this README.md are all in the same folder.
Make sure you have Streamlit installed:
   pip install streamlit
From that folder, run:
   streamlit run app.py

If streamlit isn't recognized as a command, use:

   python -m streamlit run app.py
Your browser will open the app automatically.
Features
Add an expense (date, category, description, amount)
View all expenses, with an optional category filter
View total amount spent
Category-wise summary with a bar chart
Delete an individual expense
Download your expenses.txt file
