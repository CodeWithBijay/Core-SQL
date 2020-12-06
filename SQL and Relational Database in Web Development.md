# SQL and Relational Database in Web Development

#### What is a Database?

A *database* is a set of data stored in a computer. This data is usually structured in a way that makes the data easily accessible.

#### What is a Relational Database?

A *relational database* is a type of database. It uses a structure that allows us to identify and access data *in relation* to another piece of data in the database. Often, data in a relational database is organized into tables.

#### Tables: Rows and Columns

Tables can have hundreds, thousands, sometimes even millions of rows of data. These rows are often called *records*.

Tables can also have many *columns* of data. Columns are labeled with a descriptive name (say, `age` for example) and have a specific *data type*.

For example, a column called `age` may have a type of `INTEGER` (denoting the type of data it is meant to hold).

![Table](https://content.codecademy.com/courses/sql-intensive/table.jpg)

In the table above, there are three columns (`name`, `age`, and `country`).

The `name` and `country` columns store string data types, whereas `age` stores integer data types. The set of columns and data types make up the schema of this table.

The table also has four rows, or records, in it (one each for Natalia, Ned, Zenas, and Laura).

#### What is a Relational Database Management System (RDBMS)?

A relational database management system (RDBMS) is a program that allows you to create, update, and administer a relational database. Most relational database management systems use the SQL language to access the database.

#### What is SQL?

SQL (**S**tructured **Q**uery **L**anguage) is a programming language used to communicate with data stored in a relational database management system. SQL syntax is similar to the English language, which makes it relatively easy to write, read, and interpret.

Many RDBMSs use SQL (and variations of SQL) to access the data in tables. For example, SQLite is a relational database management system. SQLite contains a minimal set of SQL commands (which are the same across all RDBMSs). Other RDBMSs may use other variants.

(SQL is often pronounced in one of two ways. You can pronounce it by speaking each letter individually like “S-Q-L”, or pronounce it using the word “sequel”.)

#### Popular Relational Database Management Systems

SQL syntax may differ slightly depending on which RDBMS you are using. Here is a brief description of popular RDBMSs:

**[MySQL](https://www.mysql.com/)**

MySQL is the most popular open source SQL database. It is typically used for web application development, and often accessed using PHP.

The main advantages of MySQL are that it is easy to use, inexpensive, reliable (has been around since 1995), and has a large community of developers who can help answer questions.

Some of the disadvantages are that it has been known to suffer from poor performance when scaling, open source development has lagged since Oracle has taken control of MySQL, and it does not include some advanced features that developers may be used to.

**[PostgreSQL](https://www.postgresql.org/)**

PostgreSQL is an open source SQL database that is not controlled by any corporation. It is typically used for web application development.

PostgreSQL shares many of the same advantages of MySQL. It is easy to use, inexpensive, reliable and has a large community of developers. It also provides some additional features such as foreign key support without requiring complex configuration.

The main disadvantage of PostgreSQL is that it can be slower in performance than other databases such as MySQL. It is also slightly less popular than MySQL.

For more information about PostgreSQL including installation instructions, read [this](https://www.codecademy.com/paths/design-databases-with-postgresql/tracks/what-is-a-database/modules/using-postgresql-on-your-own-computer/articles/installing-and-using-postgresql-locally) article.

**[Oracle DB](https://www.oracle.com/database/)**

Oracle Corporation owns Oracle Database, and the code is not open sourced.

Oracle DB is for large applications, particularly in the banking industry. Most of the world’s top banks run Oracle applications because Oracle offers a powerful combination of technology and comprehensive, pre-integrated business applications, including essential functionality built specifically for banks.

The main disadvantage of using Oracle is that it is not free to use like its open source competitors and can be quite expensive.

**[SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-2017)**

Microsoft owns SQL Server. Like Oracle DB, the code is close sourced.

Large enterprise applications mostly use SQL Server.

Microsoft offers a free entry-level version called *Express* but can become very expensive as you scale your application.

**[SQLite](https://www.sqlite.org/)**

SQLite is a popular open source SQL database. It can store an entire database in a single file. One of the most significant advantages this provides is that all of the data can be stored locally without having to connect your database to a server.

SQLite is a popular choice for databases in cellphones, PDAs, MP3 players, set-top boxes, and other electronic gadgets. The SQL courses on Codecademy use SQLite.

For more info on SQLite, including installation instructions, read [this](https://www.codecademy.com/courses/learn-sql/articles/what-is-sqlite) article.

#### Using An RDBMS On Codecademy

On Codecademy, we use both SQLite and PostgreSQL. While this may sound confusing, don’t worry! We want to stress that the basic syntax you will learn can be used in both systems. For example, the syntax to create tables, insert data into those tables, and retrieve data from those tables are all identical. That’s one of the nice parts of learning SQL — by learning the fundamentals with one RDBMS, you can easily begin work in another.

That being said, let’s take a look at some of the more subtle details:

- *File extensions* — when working with databases on Codecademy, take a look at the name of the file you’re writing in. If your file ends in `.sqlite`, you’re using a SQLite database. If your file ends in `.sql`, you’re working with PostgreSQL.

- *Data types* — You’ll learn about data types very early into learning a RDBMS. One thing to note is that SQLite and PostgreSQL have slightly different data types. For example, if you want to store text in a SQLite database, you’ll use the `TEXT` data type. If you’re working with PostgreSQL, you have many more options. You could use `varchar(n)`, `char(n)`, or `text`. Each type has its own subtle differences. This is a good example of PostgreSQL being slightly more robust than SQLite, but the core concepts remaining the same.

- *Built-in tables* — As you work your way through more complicated lessons on databases, you’ll start to learn how to access built-in tables. For example, if you take our lesson on indexes, you’ll learn how to look at the table that the system automatically creates to keep track of what indexes exist. Depending on which RDBMS system you are using (in that lesson we’re using PostgreSQL), the syntax for doing that will be different. Any time you’re writing SQL about the database itself, rather than the data, that syntax will likely be unique to the RDBMS you’re using.

  ------

  → **[PostgreSQL: What is SQL And Relational Database](https://www.youtube.com/watch?v=MZdO1UbTG4U&list=PLwvrYc43l1MxAEOI_KwGe8l42uJxMoKeS)**

  In this video, you will learn about what SQL and relational databases are. This is helpful if you want to understand the basics of SQL before delving into Postgres.

  ------

  ## Introduction to SQL

  SQL, **S**tructured **Q**uery **L**anguage, is a programming language designed to manage data stored in relational databases. SQL operates through simple, declarative statements. This keeps data accurate and secure, and helps maintain the integrity of databases, regardless of size.

  The SQL language is widely used today across web frameworks and database applications. Knowing SQL gives you the freedom to explore your data, and the power to make better decisions. By learning SQL, you will also learn concepts that apply to nearly every data storage system.

  The statements covered in this course use SQLite Relational Database Management System [(RDBMS)](https://www.codecademy.com/articles/what-is-rdbms-sql). You can also access a glossary of all the [SQL commands](https://www.codecademy.com/articles/sql-commands) taught in this course.

------

## Relational Databases

Nice work! In one line of code, you returned information from a relational database.

```
SELECT * FROM celebs;
```

We’ll take a look at what this code means soon, for now, let’s focus on what relational databases are and how they are organized.

A *relational database* is a database that organizes information into one or more tables. Here, the relational database contains one table.

A *table* is a collection of data organized into rows and columns. Tables are sometimes referred to as *relations*. Here the table is `celebs`.

A *column* is a set of data values of a particular type. Here, `id`, `name`, and `age` are the columns.

A *row* is a single record in a table. The first row in the `celebs` table has:

- An `id` of `1`
- A `name` of `Justin Bieber`
- An `age` of `22`

All data stored in a relational database is of a certain data type. Some of the most common data types are:

- `INTEGER`, a positive or negative whole number
- `TEXT`, a text string
- `DATE`, the date formatted as YYYY-MM-DD
- `REAL`, a decimal value

------

Statements

The code below is a SQL statement. A *statement* is text that the database recognizes as a valid command. Statements always end in a semicolon `;`.

```
CREATE TABLE table_name (
   column_1 data_type, 
   column_2 data_type, 
   column_3 data_type
);
```

Let’s break down the components of a statement:

1. `CREATE TABLE` is a *clause*. Clauses perform specific tasks in SQL. By convention, clauses are written in capital letters. Clauses can also be referred to as commands.
2. `table_name` refers to the name of the table that the command is applied to.
3. `(column_1 data_type, column_2 data_type, column_3 data_type)` is a *parameter*. A parameter is a list of columns, data types, or values that are passed to a clause as an argument. Here, the parameter is a list of column names and the associated data type.

The structure of SQL statements vary. The number of lines used does not matter. A statement can be written all on one line, or split up across multiple lines if it makes it easier to read. 

------

- ## Create

  `CREATE` statements allow us to create a new table in the database. You can use the `CREATE` statement anytime you want to create a new table from scratch. The statement below creates a new table named `celebs`.

  ```
  CREATE TABLE celebs (
     id INTEGER, 
     name TEXT, 
     age INTEGER
  );
  ```

  \1. `CREATE TABLE` is a clause that tells SQL you want to create a new table.
  \2. `celebs` is the name of the table.
  \3. `(id INTEGER, name TEXT, age INTEGER)` is a list of parameters defining each column, or attribute in the table and its data type:

  - `id` is the first column in the table. It stores values of data type `INTEGER`
  - `name` is the second column in the table. It stores values of data type `TEXT`
  - `age` is the third column in the table. It stores values of data type `INTEGER`

------

## Insert

The `INSERT` statement inserts a new row into a table. You can use the `INSERT` statement when you want to add new records. The statement below enters a record for Justin Bieber into the `celebs` table.

```
INSERT INTO celebs (id, name, age) 
VALUES (1, 'Justin Bieber', 22);
```

\1. `INSERT INTO` is a clause that adds the specified row or rows.
\2. `celebs` is the name of the table the row is added to.
\3. `(id, name, age)` is a parameter identifying the columns that data will be inserted into.
\4. `VALUES` is a clause that indicates the data being inserted.
`(1, 'Justin Bieber', 22)` is a parameter identifying the values being inserted.

- `1` is an integer that will be inserted into the `id` column
- `'Justin Bieber'` is text that will be inserted into the `name` column
- `22` is an integer that will be inserted into the `age` column

------

## Select

`SELECT` statements are used to fetch data from a database. In the statement below, `SELECT` returns all data in the `name` column of the `celebs` table.

```
SELECT name FROM celebs;
```

\1. `SELECT` is a clause that indicates that the statement is a query. You will use `SELECT` every time you query data from a database.
\2. `name` specifies the column to query data from.
\3. `FROM celebs` specifies the name of the table to query data from. In this statement, data is queried from the `celebs` table.

You can also query data from all columns in a table with `SELECT`.

```
SELECT * FROM celebs;
```

`*` is a special wildcard character that we have been using. It allows you to select every column in a table without having to name each one individually. Here, the result set contains every column in the `celebs` table.

`SELECT` statements always return a new table called the *result set*.

------

## Alter

The `ALTER TABLE` statement adds a new column to a table. You can use this command when you want to add columns to a table. The statement below adds a new column `twitter_handle` to the `celebs` table.

```
ALTER TABLE celebs 
ADD COLUMN twitter_handle TEXT;
```

\1. `ALTER TABLE` is a clause that lets you make the specified changes.
\2. `celebs` is the name of the table that is being changed.
\3. `ADD COLUMN` is a clause that lets you add a new column to a table:

- `twitter_handle` is the name of the new column being added
- `TEXT` is the data type for the new column

\4. `NULL` is a special value in SQL that represents missing or unknown data. Here, the rows that existed before the column was added have `NULL` (∅) values for `twitter_handle`.

------

## Update

The `UPDATE` statement edits a row in a table. You can use the `UPDATE` statement when you want to change existing records. The statement below updates the record with an `id` value of `4` to have the `twitter_handle` `@taylorswift13`.

```
UPDATE celebs 
SET twitter_handle = '@taylorswift13' 
WHERE id = 4; 
```

\1. `UPDATE` is a clause that edits a row in the table.
\2. `celebs` is the name of the table.
\3. `SET` is a clause that indicates the column to edit.

- `twitter_handle` is the name of the column that is going to be updated
- `@taylorswift13` is the new value that is going to be inserted into the `twitter_handle` column.

\4. `WHERE` is a clause that indicates which row(s) to update with the new column value. Here the row with a `4` in the `id` column is the row that will have the `twitter_handle` updated to `@taylorswift13`.

------

## Delete

The `DELETE FROM` statement deletes one or more rows from a table. You can use the statement when you want to delete existing records. The statement below deletes all records in the `celeb` table with no `twitter_handle`:

```
DELETE FROM celebs 
WHERE twitter_handle IS NULL;
```

1. `DELETE FROM` is a clause that lets you delete rows from a table.
2. `celebs` is the name of the table we want to delete rows from.
3. `WHERE` is a clause that lets you select which rows you want to delete. Here we want to delete all of the rows where the twitter_handle column `IS NULL`.
4. `IS NULL` is a condition in SQL that returns true when the value is `NULL` and false otherwise.

------

Constraints

*Constraints* that add information about how a column can be used are invoked after specifying the data type for a column. They can be used to tell the database to reject inserted data that does not adhere to a certain restriction. The statement below sets *constraints* on the `celebs` table.

```
CREATE TABLE celebs (
   id INTEGER PRIMARY KEY, 
   name TEXT UNIQUE,
   date_of_birth TEXT NOT NULL,
   date_of_death TEXT DEFAULT 'Not Applicable'
);
```

\1. `PRIMARY KEY` columns can be used to uniquely identify the row. Attempts to insert a row with an identical value to a row already in the table will result in a *constraint violation* which will not allow you to insert the new row.

\2. `UNIQUE` columns have a different value for every row. This is similar to `PRIMARY KEY` except a table can have many different `UNIQUE` columns.

\3. `NOT NULL` columns must have a value. Attempts to insert a row without a value for a `NOT NULL` column will result in a constraint violation and the new row will not be inserted.

\4. `DEFAULT` columns take an additional argument that will be the assumed value for an inserted row if the new row does not specify a value for that column.

## PostgreSQL Constraints

Introduction

In this lesson we’ll work to build out a database (DB) schema that will  store information for a conference. Our database will be designed to  accept input from a variety of applications, user filled-forms, and  other sources. We’d also like to put data validation in place to protect our DB from receiving unexpected, improperly formatted, or invalid  data.

Luckily for us, PostgreSQL offers methods to safeguard a database and maintain *data integrity*. One of these methods is called *constraints*. Constraints are rules defined as part of the data model to control what values are allowed in specific columns and tables.

Specifically, constraints:

- Reject inserts or updates containing values that shouldn’t be inserted into a  database table, which can help with preserving data integrity and  quality.
- Raise an error when they’re violated, which can help with debugging applications that write to the DB.

Let’s work towards designing a data model we might use to schedule our conference. To start, we have the  following tables with no constraints: 

- `talks` 
- `speakers`

In the next few exercises we’ll  discuss how a thoughtful implementation of the following rules and  constraints could improve our data model:

- Data types

- `NOT NULL` constraints

- `UNIQUE` constraints

- `PRIMARY KEY` constraints

- `CHECK` constraints

- `FOREIGN KEY` Constraints

  ------

  

PostgreSQL Data Types

PostgreSQL offers several ways a DB engineer can ensure that correct data is  entered into a column or table. One of the most basic methods is built  into the `CREATE TABLE` syntax that you’ve probably already seen before. 

In a `CREATE TABLE` statement we specify the *data type* for each column of a table (e.g., `int`, `text`, `timestamp`, etc.). In doing so, we’re telling PostgreSQL which types of values can  be inserted into each column in the table. You can refer to the complete list of available data types in the [PostgreSQL documentation](https://www.postgresql.org/docs/10/datatype.html).

| Name                  | Description                                                  |
| --------------------- | ------------------------------------------------------------ |
| boolean               | true/false                                                   |
| varchar or varchar(n) | text with variable length, up to n characters (if specified) |
| date                  | calendar date                                                |
| integer               | whole number value between -2147483648 and +2147483647       |
| numeric(a, b)         | decimal with total digits (a) and digits after the decimal point (b) |
| time                  | time of day (no time zone)                                   |

To create a table that stores information about volunteers for the conference we could write the following:

```
CREATE TABLE volunteers (
    id integer,
    name varchar,
    hours_available integer,
    phone_number varchar(12),
    email varchar
);
```

In the statement above, we’ve ensured that our `volunteers` table will have:

- Integer values for data in columns `id` and `hours_available` 
- Text values data in columns `name`, `phone_number`, and `email`

However, data types don’t prevent all unexpected data from being inserted into a table. For example, we’ve defined `phone_number` as `varchar(12)` and might expect a 10-digit phone number formatted as `XXX-XXX-XXXX`. Consider the following issues that may arise: 

- An incomplete value formatted like `XXX-XXXX` will be accepted because it’s under 12 characters.
- A value like `+X XXX-XXX-XXXX` will cause PostgreSQL to raise an error because it’s longer than 12 characters, even though it’s a valid entry.

Another potential issue caused by  relying only on PostgreSQL data types stems from the fact that  PostgreSQL will try to interpret incoming data as the data type the  column has been defined as. This process, called *type casting*, can have mixed results.

- If one tries to insert `1.5` into our table’s `hours_available` column, PostgreSQL will cast this value  to `integer`, round the data, and insert it into the table as `2`.
- If one tries to insert `1.5` into the `email` column, PostgreSQL will insert this into the database by casting `1.5` to `'1.5'` even though `'1.5'` is not a valid email address. 

------

 Nullability Constraints

In some cases, we might enter data into our database without including a  value for every column in each row. For example, this could happen when  aggregating data from multiple sources that don’t have the same input  columns.

Missing (`NULL`) values in certain columns might make our data much less useful. For  example, if we’re loading data into a table designed to keep a record of talks, we may want to require fields like title, session_timeslot, and  speaker_id to be filled for an entry to be valid. After all, what’s a  talk without a speaker?

Suppose we insert a row that doesn’t contain all desired fields into our current `talks` table. We can do this with the statement below.

```
INSERT INTO talks (id, estimated_length)
VALUES (1, 30);
```

We can query this table to see how this row looks when inserted into PostgreSQL when there are no constraints in place.

```
SELECT * FROM talks
WHERE id = 1;
```

| id   | title | speaker_id | estimated_length | session_timeslot |
| ---- | ----- | ---------- | ---------------- | ---------------- |
| 1    | NULL  | NULL       | 30               | NULL             |

As expected, we see that there are `NULL` values in the `title`, `session_timeslot` and `speaker_id` columns. With PostgreSQL, we can choose to reject inserts and updates that don’t include data for specific columns by adding a `NOT NULL` constraint on those columns. With this constraint in place, PostgreSQL  will reject the insert statement that contains incomplete data.  PostgreSQL will raise an error alerting us that these rows violate the  constraint and that our insert or update couldn’t be completed.

Let’s consider how we might implement this constraint on the `talks` table. If we know which columns cannot be `NULL` before creating our table, we can add a `NOT NULL` constraint following the datatype in the table’s `CREATE TABLE` statement.

```
CREATE TABLE talks (
    id integer,
    title varchar NOT NULL,
    speaker_id integer NOT NULL,
    estimated_length integer,
    session_timeslot timestamp NOT NULL
);
```

Let’s try the previous insert again.

```
INSERT INTO talks (id, estimated_length)
VALUES (1, 30);
```

Great, this statement now causes PostgreSQL to return an error. 

```pseudo
ERROR: null value in column "title"  violates not-null constraint
Detail: Failing row contains (1, null, null, 30, null).
```

The error message lets us know our  constraint is working! We even get a helpful message that shows  information about the contents of the failing row.

------

Improving Tables with Constraints

Sometimes we’ve planned out a data model and inserted data before realizing that  our model could benefit from the addition of a constraint. In  PostgreSQL, we can use `ALTER TABLE` statements to add or remove constraints from existing tables. In fact,  all of the constraints we’ll cover throughout this lesson can be added  to an existing table by writing an `ALTER TABLE` statement!

Let’s imagine we’ve already populated our `talks` table with some data, but we haven’t included any constraints. Suppose that:

- The column `session_timeslot` contains no `NULL` values
- The column `title` contains  about 50% `NULL` values 

Since we’ve already created and  inserted data into our table, we probably don’t want to re-create and  re-populate it from scratch. Instead, we can add a `NOT NULL` constraint to a column using an `ALTER TABLE` statement. Let’s add a `NOT NULL` constraint on `session_timeslot` with the following statement.

```
ALTER TABLE talks
ALTER COLUMN session_timeslot SET NOT NULL;
```

If we later decide we no longer need this constraint, we can drop a `NOT NULL` constraint from an existing table with the following statement:

```
ALTER TABLE talks
ALTER COLUMN session_timeslot DROP NOT NULL
```

If we’d like to add a `NOT NULL` constraint to the `title` column, we can attempt to do so using the same syntax we used to add a constraint on `session_timeslot`. 

```
ALTER TABLE talks
ALTER COLUMN title SET NOT NULL;
```

However, PostgreSQL will reject the addition of the constraint and raise the following error because `NULL` values are already present in the column. See the error the database returns below.

```pseudo
SQL Error [23502]: ERROR: column "title" contains null values
```

If the table we’re attempting to add a constraint on doesn’t meet the constraint, we can *backfill* the table so that it does adhere to the constraint. *Backfilling* is a term occasionally used in DB engineering to refer to the process  of adding or updating past values. In this case, we can fill our target  column’s `NULL` values with a placeholder value using the query below. 

```
UPDATE talks
SET title = 'TBD'
WHERE title IS NULL;
```

With the table updated so that there are no longer any nulls in `title`, and we can now apply the `NOT NULL` constraint.

```
ALTER TABLE talks
ALTER COLUMN title SET NOT NULL;
```

------

Introduction to Check Constraints

In some situations, we might want to establish specific rules to determine what makes a row valid. For example, In our `talks` table, we might want to ensure that the `estimated_length` column is:

- An integer
- `NOT NULL`
- Positive

The first two rules can be implemented with a data type and `NOT NULL` constraint respectively, but the third will require additional logic to enforce. We can use `CHECK` statements to implement more precise constraints on our table. A `CHECK` constraint can be written into a `CREATE TABLE` statement, or added to an existing table with `ALTER TABLE`.

To use a check constraint, we list `CHECK (...)` following the data type in a `CREATE TABLE` statement and write the condition we’d like to test for inside the parentheses. 

The condition tested for inside of parentheses of a `CHECK` statement must be a SQL statement that can be **evaluated as either true or false**. These statements are similar to the statements you may be familiar with in `WHERE` clauses when filtering rows from a table. Let’s add a `CHECK` statement to ensure our `talks` table has a positive value for `estimated_length` for each row.

```
ALTER TABLE talks 
ADD CHECK (estimated_length > 0);
```

In some situations, you may want to apply multiple constraints on a single column. In this case, we’d like to also add a `NOT NULL` constraint on `estimated_length`. We can add additional constraints on a column with multiple `ALTER TABLE` statements. 

Alternatively, If we know the  constraints we’d like to include as we’re creating a table, we can list  following the column name and datatype in a `CREATE TABLE` statement. To implement the constraints we’ve covered in this lesson you could write `estimated_length integer NOT NULL CHECK (estimated_length > 0)` into the `CREATE TABLE` statement for `talks`.

------

Check Constraints Continued

Inside a `CHECK` statement we can use a wide array of SQL syntax to create our conditions. For example, within our check constraint we can:

- Make comparisons between columns within the table
- Use logical operators like `AND` and `OR`
- Use other SQL operators you may be familiar with (`IN`, `LIKE`)

As a general rule, any logic that you might use in a `WHERE` statement to filter individual rows from an existing table can be applied within a `CHECK`, including logic that involves multiple columns or conditions. Suppose we’d like to add a check that all entries in `talks` have an `estimated_length` between 0 and 120 minutes. We could apply such a check with the following:

```
ALTER TABLE talks 
ADD CHECK (estimated_length > 0 AND estimated_length < 120);
```

We can also apply constraints that apply to multiple columns. For example, suppose we want to enforce the following:  

1. `estimated_length` less than 120 minutes 
2. year of the talk should be 2020 (we can extract this value from `session_timeslot`) 

We could do this by adding separate checks on each of the columns. Alternatively, we could add a single `CHECK` constraint that checks both conditions as shown below. 

```
ALTER TABLE talks
ADD CHECK (estimated_length < 120 AND date_part('year', session_timeslot) = 2020);
```

Don’t worry if you’re not familiar with this syntax, the `date_part` function in PostgreSQL just returns a portion of the date as an integer (e.g. `date_part('year' ,'2020-08-01 00:00:00'::date)` = 2020). 

------

Using Unique Constraints

When designing a PostgreSQL data model, it’s a good practice to structure  tables such that rows are uniquely identifiable by some combination of  attributes. Structuring your tables in this way leads to a few benefits:

- The structure of your data model and the contents of individual tables are more easily interpreted.
- Queries to access information from the table can be simpler. For example, if we’d like to query our `attendees` table to find out how many tickets an attendee has reserved, having a  unique identifier for each attendee allows us to get a result without  any intermediate aggregation.
- Identifying and implementing a `PRIMARY KEY` is easier on tables with `UNIQUE` constraints already in place.

In our `attendees` table, suppose that we’d like to make sure that no two people submit  the same email address when they register. To do so we could apply a  unique constraint on `email`.

To implement this constraint we could include it in our `CREATE TABLE` statement. To identify values in a single column as unique, we specify `UNIQUE` following the column name and datatype definitions, in this case we’d write `email varchar UNIQUE` in our `CREATE TABLE` statement.

Alternatively, we can add the constraint to an existing table using the following:

```
ALTER TABLE attendees 
ADD UNIQUE (email);
```

Returning to our `talks` table, suppose we’d like to use the combination of `speaker_id` and `session_timeslot` to ensure that a speaker is never booked for multiple talks at the same time. We can do this in the `CREATE TABLE` statement by specifying the columns that need to be jointly unique in  parentheses on its own line following the column names and datatype  definitions. In this case, we’d add a `UNIQUE (speaker_id, session_timeslot)` on it’s own line in the `CREATE TABLE` statement.

Just as with single column unique constraints, we can also  and add the constraint with an `ALTER TABLE` statement.

```
ALTER TABLE talks
ADD UNIQUE (speaker_id, session_timeslot)
```

------

Introduction to Primary Keys

Having unique constraints is useful, but an important part of building a  relational data model requires defining relationships between tables. *Primary keys* are essential to defining these relationships.

A primary key is a column (or set of columns) that **uniquely identifies a row within a database table**. A table can only have one primary key, and in order to be selected as a primary key a column (or set of columns) should:

- Uniquely identify that row in the table (like a `UNIQUE` constraint)
- Contain no null values (like a `NOT NULL` constraint)

Implementing a `PRIMARY KEY` constraint is similar to simultaneously enforcing a `UNIQUE` and `NOT NULL` constraints on a column (or set of columns). Although `UNIQUE NOT NULL` and `PRIMARY KEY` constraints function very similarly, tables are limited to one `PRIMARY KEY`, but not limited in how many columns can have both `UNIQUE` and `NOT NULL` constraints.

In addition to defining relationships between tables, primary keys also improve your data model in several other ways:

- Many joins will use the primary key from one table to join data with another table
- Primary keys can improve query performance
- Primary keys help to enforce data integrity within a table by ensuring that rows can be uniquely identified    

Recall that the `attendees` table has a column named `id` that uniquely identifies attendees. We have also already restricted the `name` and `email` columns to be `NOT NULL`“. Now let’s add `id` as our table’s `PRIMARY KEY`, we can do this with an `ALTER TABLE` statement. 

```
ALTER TABLE attendees
ADD PRIMARY KEY (id); 
```

Even with a primary key, there’s still good reason to use a combination of `UNIQUE` and `NOT NULL` constraints to enforce data integrity on other columns. In this case, the combination of a `UNIQUE` and `NOT NULL` constraint on `email` can be used to validate that all attendees have a value for `email` and each unique email can only be matched to one attendee. 

Now that you’re familiar with how  primary keys work, for the remainder of the lesson, you may assume that  all tables in our data model have a primary key on their `id` column.

------

Introduction To Foreign Keys

Let’s use some of what we’ve learned so far about primary keys to improve `registrations`. Recall the `registrations` table that we previously created had an `id` primary key column, and had fields `attendee_id`, `session_timeslot` jointly unique, so that no attendee may register for two talks with the same timeslot.

In this model, the talks in `registrations` are meant to reference the talks described in `talks`. Because of this, we’d probably want to ensure that any `talk_id` entered into `registrations` references an `id` that already appears in `talks`. 

When discussing relations between tables, you may see the terms *parent table* and *child table* to describe two tables that are related. More specifically, values inserted into *child table* must be validated by data that’s already present in a *parent table*. 

Formally, this property that ensures data can be validated by referencing another table in the data model is called *referential integrity*. Referential integrity can be enforced by adding a `FOREIGN KEY` on the child table that references the primary key of a parent table.

If the parent table doesn’t contain the data a user is attempting to insert, PostgreSQL will reject the  insert or update and throw an error. 

Let’s work through the example described above to improve `registrations`. In our example above `registrations` is a child table of `talks` because entries in `registrations` must reference the primary key from `talks`. Suppose `talks` also has a column named `id` ad a primary key. Now, we can update our registrations table with a foreign key using the following statement.

```
ALTER TABLE registrations
ADD FOREIGN KEY (talk_id)
REFERENCES talks (id);
```

Alternatively, if we’re creating a table from scratch, we can include the following line in the `CREATE TABLE` statement , `FOREIGN KEY (talk_id) REFERENCES talks (id)`

Suppose we now want to enter a registration for `talk_id = 100`, which does not yet exist in the `talks` table. Trying to insert a registration for this talk yields an error because there is not a corresponding entry in `talks` to reference yet. The error below lets us know the constraint is  working and provides a helpful error message that indicates we need to  add an entry to `talks` before this insert will succeed.

```
INSERT INTO registrations VALUES (100, 1, '2020-08-15 9:00:00', 1);
SQL Error [23503]: ERROR: insert or update on table "registrations" violates foreign key constraint "registrations_id_fkey"
Detail: Key (talk_id)=(100) is not present in table "talks".
```

------

Foreign Keys - Cascading Changes

In the previous lesson we discussed how foreign keys enforce referential  integrity by preventing updates or deletes on the parent table until the child table is updated first. An engineer can specify the strategy  PostgreSQL will use to maintain referential integrity as they define  their foreign key constraint.

By default, a foreign key  constraint will prevent an engineer from deleting or updating a row of a parent table that is referenced by some child table. This behavior is  sometimes explicitly specified in a `CREATE TABLE` statement using `REFERENCES talks (id) ON DELETE RESTRICT` or `REFERENCES talks (id) ON UPDATE RESTRICT`. 

However, another strategy you may consider is adding a `CASCADE` clause. Rather than preventing changes, `CASCADE` clauses (`ON UPDATE CASCADE`, `ON DELETE CASCADE`) **cause the updates or deletes to automatically be applied to any child tables**.

For example, suppose we’d like to  set up our database to automatically unregister attendees from a talk  that’s been cancelled. To do this we could  apply `ON DELETE CASCADE` to our foreign key constraint.

```
ALTER TABLE registrations
ADD FOREIGN KEY (talk_id)
REFERENCES talks (id) ON DELETE CASCADE
```

When we try to delete a value from `talks`, we also notice that all registrations for talk_id = 1 are removed as  well. This preserves referential integrity by removing any row  associated with this talk. To demonstrate, let’s first return the rows  in `registrations` for `talk_id` = 1.

```
SELECT * 
FROM registrations
WHERE talk_id = 1;
```

| id   | attendee_id | session_timelot    | talk_id |
| ---- | ----------- | ------------------ | ------- |
| 8    | 2           | 2020-08-15 9:00:00 | 1       |
| 9    | 5           | 2020-08-15 9:00:00 | 1       |
| 10   | 8           | 2020-08-15 9:00:00 | 1       |
| 11   | 9           | 2020-08-15 9:00:00 | 1       |
| 12   | 10          | 2020-08-15 9:00:00 | 1       |
| 13   | 11          | 2020-08-15 9:00:00 | 1       |
| 14   | 3           | 2020-08-15 9:00:00 | 1       |

Great, we observe 7 registrations for `talk_id = 1` in `registrations`. Now, let’s use the following code to delete the talk with `id = 1`:

```
DELETE FROM talks 
WHERE id = 1;
```

Because we’ve specified `ON DELETE CASCADE` on our foreign key, the `DELETE` statement ran successfully even though there were still rows in `registrations` that referenced `talk_id = 1`. Let’s check to see what affect this statement had on `registrations`.

```
SELECT * 
FROM registrations
WHERE talk_id = 1;
```

|  id  | attendee_id | session_timelot | talk_id |
| :--: | :---------: | :-------------: | :-----: |
|      |             |                 |         |

As expected, records that correspond to `talk_id = 1` have been removed. In effect, `ON DELETE CASCADE` runs the required deletes on the child table behind the scenes and  allows the user to simply run a single command to update a data model.