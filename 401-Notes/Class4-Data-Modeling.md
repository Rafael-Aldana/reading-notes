# Data Modeling

## nosql vs sql

What type of database is the best fit for the complex query intensive environment?

For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

What type of database is the best fit for hierarchical data storage?

For the type of data to be stored: SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

SQL databases are good at handling structured data, which means data that has a consistent format and is organized into tables with predefined columns. SQL databases are very good at handling complex queries and transactions, but they can be limited in their ability to scale horizontally, which means adding more servers to handle increasing amounts of data and users. This is because SQL databases have a fixed schema, which can make it difficult to add new data types or change the structure of existing data.

On the other hand, NoSQL databases are good at handling unstructured or semi-structured data, which means data that doesn't fit neatly into a table. NoSQL databases are highly scalable and can easily handle large amounts of data and users. They are also very flexible, which means you can add new data types or change the structure of existing data without worrying about the fixed schema of an SQL database.

## sql modeling techniques

Among data tables, what is a one-to-many relationship and how do we “relate” them?

We connect lines between tables to show relationships.  In some cases an entry in one table can be related to more than one entry in another.  This is called a one-to-many relationship.  In our example there are many employees in on department; therefore, we show a many-to-one relationship.

A many-to-one relationship is similar to a one-to-many relationship, this difference is in the point-of-view you take when naming the relationship.  I think most people speak of  one-to-many relationship more often.

Sometimes a there may not be an entry in a table, so technically speaking the you could have zero or one to many, but that gets hard to say, so when speaking in general terms, most people say “one-to-many.”  However, when you want to get precise,   you can use notation to specify the cardinality of a relationship.

Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

When working with SQL databases it is often useful to create diagrams of the database tables and their relationships.

Explain the difference between a primary and foreign key.

A primary key is used to identify unique rows in a table, while a foreign key is used to define a relationship between tables. The primary key is used as a reference in the foreign key of another table, which ensures that the data in both tables is consistent and accurate.

## sql vs nosql

How do we treat keywords and parameters differently in SQL syntax?

In SQL syntax, keywords and parameters are treated differently.

Keywords are reserved words that have a specific meaning in SQL, and they are used to define the structure and operations of a database. Examples of keywords in SQL include SELECT, FROM, WHERE, INSERT, UPDATE, DELETE, and JOIN. Keywords are not case sensitive in SQL, which means that you can write them in uppercase or lowercase letters.

Parameters, on the other hand, are values that are passed to SQL statements to filter or manipulate data. Parameters can be used in place of specific values in SQL statements, and they are denoted by a placeholder symbol, typically a question mark (?) or a colon followed by a parameter name (:param). Parameters are used to make SQL statements dynamic, which means that the same statement can be reused with different values. Parameters are case sensitive in SQL, and their names must follow the naming rules of SQL identifiers.

In summary, keywords are used to define the structure and operations of a database in SQL, while parameters are used to pass values to SQL statements to filter or manipulate data. Keywords are reserved words in SQL and are not case sensitive, while parameters are values that are denoted by a placeholder symbol and are case sensitive.

Define normalization within the context of schemas and data.

Normalization is a process of organizing data in a database by eliminating redundant data and ensuring that each piece of data is stored in only one place. The goal of normalization is to minimize data redundancy and increase data consistency, which leads to better database performance, easier maintenance, and more efficient data retrieval.

In the context of database schemas, normalization involves dividing the data into multiple related tables and establishing relationships between them using primary and foreign keys. The process of normalization typically involves a set of rules called normal forms, which define the level of normalization achieved by a database schema.

The most commonly used normal forms are first normal form (1NF), second normal form (2NF), and third normal form (3NF). First normal form requires that each column in a table contains only atomic values, which means that there are no repeating groups or arrays of data. Second normal form requires that every non-key column in a table is functionally dependent on the primary key, which means that there are no partial dependencies. Third normal form requires that every non-key column in a table is dependent only on the primary key, which means that there are no transitive dependencies.

Overall, normalization is an important process in database design that helps to ensure data consistency and eliminate data redundancy, leading to more efficient and effective database management.

Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

A one-to-one relationship means one record is linked to only one record in another table, a one-to-many relationship means one record in one table is linked to one or more records in another table, and a many-to-many relationship means one record in one table is linked to one or more records in another table, and vice versa, using a third junction table.

[link-to-reading-notes](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool).
[link-to-reading-notes](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/).
[link-to-reading-notes](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y).

## Bookmark and Review

[link-to-reading-notes](https://sequelize.org/master/).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?