## My summary of reading the SQL part.
# **What is SQL:**

![SQL](https://swansoftwaresolutions.com/wp-content/uploads/2020/03/07.30.20-The-Importance-of-SQL-Skills-for-Software-Testers-1024x576.jpg)

It stands for (Structured Query Language) and it's a language that has been designed to manipulate and transform data from where they have been stored it's well known for providing large data storage spaces and it's relativley safe to store information in and retrieve later on from it.

# **Realtional data bases:**

It represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.


# **SQL queries:**

1- Select: It is used to retrieve data from the table 
   Syntax:(SELECT column, another_column, …
        FROM TableNmae;).

2- Constraints on queries(conditions) PT1: Are used when we need to specify or retrieve specific values not the whole thing.
Syntax: (SELECT column, another_column, …
FROM TableName
WHERE condition
    AND/OR another_condition
    AND/OR …;)

3- Constraints on queries(conditions) PT2: You can have multiple conditions inside one another
Syntax: (SELECT column, another_column, …
FROM TableName
WHERE condition
    AND/OR another_condition
    AND/OR …;)    

# ** Filtering and sorting query results:**

1- Using (DISTINCT): It is used to remove duplicate rows.
  Syntax:(SELECT DISTINCT column, another_column, …
FROM TableName
WHERE condition(s);)

2- Using (Order by): It is used to order query results especially when having a large table
Syntax (SELECT column, another_column, …
FROM TableName
WHERE condition(s)
ORDER BY column ASC/DESC;) 

3- Limiting results to subsets: which is a useful optimization to indicate to the database the subset of the results you care about.
Syntax(SELECT column, another_column, …
FROM TableName
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;)

# **What is a schema?**
It is what describes the structure of each table, and the datatypes that each column of the table can contain.

# **Inserting a row:**
When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. 
Syntax:(INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;)


# **Updating rows:**
Update existing data can be done using an UPDATE statement.
Where  you have to specify exactly which table, columns, and rows to update. In addition, the data you are updating has to match the data type of the columns in the table schema.
Syntax:(UPDATE TableName
SET column = value_or_expr, 
other_column = another_value_or_expr, …
WHERE condition;)

# **Deleting rows:**
When you need to delete data from a table in the database, you can use a DELETE statement, which describes the table to act on, and the rows of the table to delete through the WHERE clause.'
Syntax:(DELETE FROM TableName
WHERE condition;)

# **Creating tables:**
The structure of the new table is defined by its table schema, which defines a series of columns. Each column has a name, the type of data allowed in that column, an optional table constraint on values being inserted, and an optional default value.
Syntax:(CREATE TABLE TableName (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value…
);)

# **Dropping a table:**
you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.
Syntax:(DROP TABLE IF EXISTS mytable;)

![NodeJS](https://www.researchgate.net/profile/Sameem-Abdul-Kareem/publication/277736380/figure/fig2/AS:669387052826625@1536605718015/Flowchart-for-translation-to-SQL-statement.png)

# And that was it for this summary.