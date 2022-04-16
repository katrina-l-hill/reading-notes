# SQL Practice – Reading Notes for e-book and SQL Bolt tutorial

## Learn SQL e-book

### Basic SQL

- The SELECT statement is the most simple statement in SQL and the first place to start with any query.  
- The FROM statement allows you to specify the location to which you want to retrieve data in the tables.  
- To get all data out of all the columns in a database, you could use the asterisk (*) clause following the SELECT statement.  
- The ORDER BY statement allows you to sort data returned from the database.  
- One common way to sort data is using the ascending (ASC) and descending (DESC) clauses.  
- The LIMIT statement allows you to place a limit on the number of rows returned from the query. It also allows the data to return back faster since you’re limiting the amount of data being returned.  
- The OFFSET statement allows you to select a starting point in the database from which to return data.  
- A SCHEMA is a collection of tables and relationships in a database.  
- The rows, or instances, in a database can have different schemas.  

### Mid-Level SQL

- The WHERE statement is used to place conditions by which to filter. The conditions are either true or false.  
- These conditions include AND, OR, and NOT.  
- Conditions also use the order of operations such as that in mathematics to return data.  
- Operators used in SQL include = (equal), < (less than), > (greater than), <= (less than or equal to), >= (greater than or equal to), != (not equal), <> (not equal), string operators (LIKE (a string matches a pattern: -, %), ILIKE (case insenstive version of LIKE), SIMILAR TO (a string matches a regex pattern).  
- The NULL clause is used to return data that where cells are or are not null. The following conditions are used: IS NULL (matches NULL values) and IS NOT NULL (matches all non NULL values).  
- Aggregate Functions are functions used to handle the data once it’s returned.  
- These functions include COUNT and GROUP BY.  
- The COUNT function returns how many of something you specify.  
- The DISTINCT clause is used with the COUNT function  to tally the number of unique values in the data.  
- The GROUP BY function splits the returned aggregate data into groups.  
- The JOIN function allows you to group tables together by keys (i.e., ids) that are the same across different tables.  
- The JOIN function has different types. These are INNER, LEFT OUTER, RIGHT OUTER, and FULL OUTER.  
- The INNER JOIN type will return all data in a row that matches the queried data.  
- The LEFT OUTER JOIN returns all data in a row that matches from the left listed table.  
- The RIGHT OUTER JOIN returns all data in a row that matches from the right listed table.  
- The FULL OUTER JOIN returns all data in a row that matches from both tables.  

## SQL Bolt tutorial

### Intro to SQL

- Structured Query Language (SQL) is a language that allows you to use relational databases to query, manipulate, and transform data.  
- A relational database is where data is structured related tables. The database has scalable storage and can store data for millions of applications.  

### Lesson 1: SELECT queries 101

- Writing a SELECT query, or statement, allows you to retrieve data from a SQL database.  
- When you write a query, you’re trying to find out what data you’re looking for, where the data is located in the database, and potentially how to transform the data type before it’s returned.  
- When querying data to be returned, you can select specific columns (properties) and rows (instances of the entity).  
- In addition, to retrieve all the data in properties, you can use the asterisk (*). Using the asterisk allows you to view all the data at once.  

### Lesson 2: Queries with constraints (Pt. 1)

- Using a WHERE clause in the query allows you to filter through data to return specific results from the database.  
- WHERE will be applied to each row and column to filter for the specific results.  
- Clauses can reduce the amount of data returned, thereby making the query run faster and the data returned faster as well.  
- There are additional clauses or operators to filter data. These include standard numerical operators, BETWEEN … AND …, NOT BETWEEN … AND …, IN (…), and NOT IN (…).  

### Lesson 3: Queries with constraints (Pt. 2)

- WHERE clauses can query for case-sensitive and case-insensitive string data using specific operators.  
- Case sensitive operators include =, !=, or <, >.  
- Case insensitive operators include LIKE and NOT LIKE.  
- Strings must be enclosed in quotes for the query to parse the data and identify where it’s a string or an SQL keyword.  

### Lesson 4: Filtering and sorting Query results

- The DISTINCT keyword allows you to filter out duplicate rows with the same values.  
- You can use the ORDER BY clause to sort data in columns in ascending or descending alpha-numeric order.  
- The further filter data through a query, you can use the LIMIT and OFFSET clauses. LIMIT reduces the number of rows that are returned from a specified row to start the query from, OFFSET.  
- These clauses are applied after other clauses have been set.  

### Lesson 6: Multi-table queries with JOINs

- Normalization in a SQL database is a process by which duplicate data is minimized so that redundancy is eliminated.  
- By normalizing data in a database, you allow data to grow in the table independently of data in other tables.  
- Normalizing the data can lead to reduction in performance and speed that the data is returned because queries have to cross tables to locate data to return.  
- Using the JOIN clause can help make the query faster and easier by combining row data across separate tables. To do this, a unique key is given to each entity in a table when data is shared.  

### Lesson 13: Inserting rows

- A schema describes the structure of each table in a database, as well as the data types in each column.  
- The schema ensures the data is consistent across the tables.  
- The INSERT statement is used to insert new data into the database.  
- This statement will declare the table the data will go into, the columns to be filled, and the number of rows that are being inserted.  
- It’s best practice to ensure every new row being inserted contains a value that corresponds with a column in the table.  

### Lesson 14: Updating rows

- The UPDATE statement updates existing data in the database.  
- You will need to declare the table the data will go into, and the columns and rows that are being updated.  
- Most importantly, the data being updated has to match the data type that’s in the schema.  
- Forgetting to add the WHERE clause when updating existing data will cause you to update all rows instead of specific ones.  
- To help alleviate this potential error, you can test the UPDATE statement in a SELECT query to update the column data as desired.  

### Lesson 15: Deleting rows

- The DELETE statement deletes data from a database table.  
- You need to specify the table or rows that need to be completed by using the WHERE clause.  
- You will need to ensure the WHERE clause is included or all rows will be deleted.  
- As with the UPDATE statement, you can test the DELETE statement in a SELECT query to update the column data as desired.  
- Try to remember to review the DELETE statement twice so that you only have to execute it once.  

### Lesson 16: Creating tables

- The CREATE TABLE statement allows you to add a new table to a database.  
- You will need to insert data into the new table that meets the same data types as in the schema.  
- To ensure you’re not trying to insert a new table with columns and tables that already exist, use the IF NOT EXISTS clause with the CREATE TABLE statement.  
- Common database data types are INTEGER, BOOLEAN, CHARACTER(num_chars), VARCHAR(num_chars), TEXT, and BLOB.  
- The different types of table constraints include PRIMARY KEY, UNIQUE, CHECK (expression), and FOREIGN KEY.  

### Lesson 17: Altering tables

- The ALTER TABLE statement is used to add, remove, or modify column and table constraints.  
- To add a new column, use the ADD clause and type the name of the new table following “column.”  
- To remove a column, use the DROP clause and type the name of the column to be deleted.  
- To rename a table, use the RENAME TO clause along with the ALTER NAME statement.  

### Lesson 18: Dropping tables

- The DROP TABLE statement is used to completely delete an entire table and it’s data as well as the schema.  
- A potential issue with deleting a table and schema is that there could be dependent data in other tables that use the data being deleted. You will need to remove the connection between the dependent table or remove the dependent table as well.  

#### Screenshots of Completed Task Lists

[Task List 1](./assets/img/bolt-task-1.png)  
[Task List 2](./assets/img/bolt-task-2.png)  
[Task List 3](./assets/img/bolt-task-3.png)  
[Task List 4](./assets/img/bolt-task-4.png)  
[Task List 5](./assets/img/bolt-task-5.png)  
[Task List 6](./assets/img/bolt-task-6.png)  
[Task List 13](./assets/img/bolt-task-13.png)  
[Task List 14](./assets/img/bolt-task-14.png)  
[Task List 15](./assets/img/bolt-task-15.png)  
[Task List 16](./assets/img/bolt-task-16.png)  
[Task List 17](./assets/img/bolt-task-17.png)  
[Task List 18](./assets/img/bolt-task-18.png)