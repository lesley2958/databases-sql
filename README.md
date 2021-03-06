Intro to Databases & SQL
==================

Brought to you by [Lesley Cordero](http://www.columbia.edu/~lc2958).

## Table of Contents

- [0.0 Setup](#00-setup)
	+ [0.1 Python and Pip](#01-python-and-pip)
	+ [0.2 Modules](#02-modules)
- [1.0 Background](#10-background)
	+ [1.1 What is a database?](#11-what-is-a-database)
		* [1.1.1 What is a relational database?](#111-what-is-a-relational-database)
		* [1.1.2 What is a table?](#112-what-is-a-table)
	+ [1.2 What is a clause?](#12-what-is-a-clause)
	+ [1.3 What is a schema?](#13-what-is-a-schema)
- [2.0 SQL](#20-sql)
	+ [2.1 What is SQL?](#21-what-is-sql)
	+ [2.2 Building a Database](#22-building-a-database)
	+ [2.3 Inserting](#23-inserting)
	+ [2.4 Selecting](#24-selecting)
	+ [2.5 Updating](#25-updating)
	+ [2.6 Deleting](#26-deleting)
	+ [2.7 Null](#27-null)
	+ [2.8 Aggregations](#28-aggregations)(#28-aggregations)
	+ [2.9 Subqueries](#29-subqueries)
		* [2.9.1 2D Tables](#291-2d-tables)
		* [2.9.2 1D Arrays](#292-1d-arrays)
		* [2.9.3 Single Values](#293-single-values)
- [5.0 Final Words](#50-final-words)
	+ [5.1 Resources](#51-resources)
	+ [5.2 More!](#52-more)


## 0.0 Setup

This guide was written in Python 3.5.


### 0.1 Python and Pip

Download [Python](https://www.python.org/downloads/) and [Pip](https://pip.pypa.io/en/stable/installing/).

### 0.2 Modules

```
pip3 install sqllite3
```

## 1.0 Background

### 1.1 What is a database?

#### 1.1.1 What is a relational database?

 A relational database is a database that organizes information into one or more tables. 

#### 1.1.2 What is a table? 

A table is a collection of data organized into rows and columns. Tables are sometimes referred to as relations.


### 1.2 What is a clause?

Clauses perform specific tasks in SQL. By convention, clauses are written in capital letters. Clauses can also be referred to as commands.

### 1.3 What is a schema?


## 2.0 SQL


### 2.1 What is SQL? 


### 2.2 Building a Database

The structure of SQL statements vary. The number of lines used do not matter. A statement can be written all on one line, or split up across multiple lines if it makes it easier to read. In this course, you will become familiar with the structure of common statements.

``` SQL
CREATE TABLE table_name (
    column_1 data_type, 
    column_2 data_type, 
    column_3 data_type
  );
```

### 2.3 Inserting

`INSERT INTO` is a clause that adds the specified row or rows. 

``` SQL
INSERT INTO table (id, name, age) VALUES (1, 'Lesley Cordero', 25);
```

### 2.4 Selecting

``` SQL
SELECT * FROM celebs;
```
`SELECT` statements are used to fetch data from a database. `SELECT` is a clause that indicates that the statement is a query. You will use `SELECT` every time you query data from a database. `SELECT` statements always return a new table called the result set. We can also rename the columns we want to show with `AS`.

`*` is a special wildcard character that we have been using. It allows you to select every column in a table without having to name each one individually. Here, the result set contains every column in the celebs table.

### 2.5 Updating

The `UPDATE` statement edits a row in the table. You can use the UPDATE statement when you want to change existing records. `SET` is a clause that indicates the column to edit. WHERE is a clause that indicates which row(s) to update with the new column value.

The `ALTER TABLE` statement added a new column to the table. You can use this command when you want to add columns to a table. `ADD COLUMN` is a clause that lets you add a new column to a table. 

### 2.6 Deleting

The `DELETE` FROM statement deletes one or more rows from a table. You can use the statement when you want to delete existing records.

### 2.7 Null

`NULL` is a special value in SQL that represents missing or unknown data. Here, the rows that existed before the column was added have NULL values for twitter_handle

### 2.8 Aggregations

Aggregations are used to convert many rows into a single row. Almost all aggregations come with the `GROUP BY` statement, which converts the table otherwise returned by the query into groups of tables. Each group corresponds to a unique value (or group of values) of columns which we specify in the GROUP BY statement.


### 2.9 Subqueries 

Subqueries are regular SQL queries that are embedded inside larger queries. There are 3 different types of subqueries, based on what they return -


#### 2.9.1 2D Table 

#### 2.9.2 1D Array

#### 2.9.3 Single Values


## 5.0 Final Words


### 5.1 Resources

[]() <br>
[]()

### 5.2 Mini Courses

Learn about courses [here](www.byteacademy.co/all-courses/data-science-mini-courses/).

[Python 101: Data Science Prep](https://www.eventbrite.com/e/python-101-data-science-prep-tickets-30980459388) <br>
[Intro to Data Science & Stats with R](https://www.eventbrite.com/e/data-sci-109-intro-to-data-science-statistics-using-r-tickets-30908877284) <br>
[Data Acquisition Using Python & R](https://www.eventbrite.com/e/data-sci-203-data-acquisition-using-python-r-tickets-30980705123) <br>
[Data Visualization with Python](https://www.eventbrite.com/e/data-sci-201-data-visualization-with-python-tickets-30980827489) <br>
[Fundamentals of Machine Learning and Regression Analysis](https://www.eventbrite.com/e/data-sci-209-fundamentals-of-machine-learning-and-regression-analysis-tickets-30980917759) <br>
[Natural Language Processing with Data Science](https://www.eventbrite.com/e/data-sci-210-natural-language-processing-with-data-science-tickets-30981006023) <br>
[Machine Learning with Data Science](https://www.eventbrite.com/e/data-sci-309-machine-learning-with-data-science-tickets-30981154467) <br>
[Databases & Big Data](https://www.eventbrite.com/e/data-sci-303-databases-big-data-tickets-30981182551) <br>
[Deep Learning with Data Science](https://www.eventbrite.com/e/data-sci-403-deep-learning-with-data-science-tickets-30981221668) <br>
[Data Sci 500: Projects](https://www.eventbrite.com/e/data-sci-500-projects-tickets-30981330995)
