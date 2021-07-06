# SQL

## Complete SQLBolt

**What is SQL?**

  SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

  Before learning the SQL syntax, it's important to have a model for what a relational database actually is. A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

  To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. It has a specific syntax though, which is what we are going to learn in the following exercises.

  Even though the data in a database may be unique, the results of any particular query may not be – take our Movies table for example, many different movies can be released the same year. In such cases, SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.

## A Primer on SQL

  A **database** is nothing but a collection of organized data. It doesn’t have to be in a digital format to
  be called a database. A telephone directory is a good example, which stores data about people and
  organizations with a contact number. Software which is used to manage a digital database is called
  a **Database Management System (DBMS)**.

  The most prevalent database organizational model is the **Relational Model**, developed by Dr. E F
Codd in his groundbreaking research paper - A Relational Model of Data for Large Shared Data
Banks.In this model, data to be stored is organized as rows inside a table with the column headings
specifying the corresponding type of data stored. This is not unlike a spreadsheet where the first
row can be thought of as column headings and the subsequent rows storing the actual data.

SQL stands for **Structured Query Language** and it is the de-facto standard for interacting with
relational databases. Almost all database management systems you’ll come across will have a SQL
implementation. SQL was standardized by the American National Standards Institute (ANSI) in
1986 and has undergone many revisions, most notably in 1992 and 1999. However, all DBMS’s do
not strictly adhere to the standard defined but rather remove some features and add others to provide
a unique feature set. Nonetheless, the standardization process has been helpful in giving a uniform
direction to the vendors in terms of their database interaction language.

## SQL Cheat Sheet

  This cheatsheet has a list of commands to be used with SQL.

