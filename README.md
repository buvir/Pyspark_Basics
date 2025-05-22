# PySpark Basics on Databricks

This repository contains a Databricks notebook titled Pyspark_Basics that demonstrates the fundamentals of working with PySpark in a distributed computing environment.

📌 Overview
This notebook was developed on Databricks and covers the core concepts of PySpark, including:

Creating Spark sessions

Working with RDDs and DataFrames

Basic transformations and actions

Reading and writing data (CSV, JSON)

Data analysis using Spark SQL

This Jupyter notebook (Pyspark_Basics (1).ipynb) demonstrates basic PySpark operations using the Titanic dataset. The notebook includes data loading, display, and simple SQL queries executed in a Databricks environment.

🚀 Environment
Platform: Databricks

Language: Python (PySpark)

Cluster Mode: Single Node / Community Edition compatible

Contents
Data Loading: The notebook loads the Titanic dataset from a SQL table named titanic_3_csv using sqlContext.sql.

Data Display: The dataset is displayed in two ways:

Using .show() to print the first 20 rows in a tabular format.

Using display() to render an interactive table in the Databricks notebook.

Key Features
PySpark SQL: The notebook uses PySpark SQL to query and display data.

Databricks Integration: The notebook is designed to run in a Databricks environment, as indicated by the metadata and the use of display().

Usage
Environment: Ensure you are running this notebook in a Databricks environment with PySpark installed.

Data Source: The notebook assumes the Titanic dataset is available in a table named titanic_3_csv.

Execution: Run the cells sequentially to load and display the dataset.

Example Code
python
# Load data from SQL table
df = sqlContext.sql("Select * from titanic_3_csv").show()

# Display data in Databricks notebook
display(df)
Notes
The dataset includes passenger details such as PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, and Embarked.

The notebook is part of a PySpark basics tutorial, focusing on data loading and display operations.
