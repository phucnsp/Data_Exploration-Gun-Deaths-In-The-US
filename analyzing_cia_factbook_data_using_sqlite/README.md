# Analyzing_CIA_Factbook_Data_Using_SQLite_and_Python

In this project, we'll work with data from the CIA World Factbook, a compendium of statistics about all of the countries on Earth. The Factbook contains demographic information like:
- population - The population as of 2015.
- population_growth - The annual population growth rate, as a percentage.
- area - The total land and water area.

We'll explore the Python SQLite workflow to explore, analyze, and visualize data from this database. 
We'll connect to a SQLite database and query it using the `sqlite3` module. When working in the Jupyter notebook environment, we can actually use pandas to run SQL queries and display the results neatly as a DataFrame object. We create a sqlite3.Connection instance as usual and then use pandas.read_sql_query(sql, con) to handle running the query and returning the results in a table.
```python
  import sqlite3
  import pandas as pd
  conn = sqlite3.connect("factbook.db")

  q = "SELECT * FROM sqlite_master WHERE type='table';"
  pd.read_sql_query(q, conn)
```

If we had used the default sqlite3 querying method, we would have gotten back nested tuples.

You may be wondering why we're using SQLite at all if we're just reading in the results into pandas dataframes anyway. Why not just use pandas? Most data analysts and data scientists in industry use a SQL GUI based tool which:
  -let you write queries and save them for later
  -let you run queries against multiple enterprise database systems (MySQL, Postgres, etc.)
  -return results as a table
  -create standard visualizations like line charts, bar plots, and histograms from the results table without any programming
