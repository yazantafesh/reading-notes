# Data Modeling

## Review, Research, and Discussion

1- **Name 3 advantages to Test Driven Development**

- reduce the time required for project development.
- save project costs in the long run.
- code flexibility and easier maintenance.

2- **In what case would you need to use beforeEach() or afterEach
() in a test suite?**

- in an instance where tests should be explicit
- when tests should never share the same state between tests

3- **What is one downside of Test Driven Development**

  Tests have to be maintained when requirements change.

4- **What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

  A class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

5- **Why REST?**

  The WRRC is inherently stateless. Using REST creates states - which is like creating knowledge of actions that happened before the client made the request and what will or should happen after the response is sent back to the client. REST is used when you are talking to your API (vs. CRUD which is used when you are talking to a database).

## Document the following Vocabulary Terms

- **functional programming** is a way of thinking about software construction by creating pure functions.

- **object-oriented programming (OOP)** is a computer programming model that organizes software design around data, or objects, rather than functions and logic.

- **class** is a blueprint for creating objects.

- **super** is the parent class of the derived one.

- **this** is a reserved keyword in JS that is a pointer to the current object you are using.

- **Test Driven Development (TDD)** a software development approach where we write the tests before the code.

- **Jest** is a JavaScript testing framework maintained by Facebook for tests and such.

- **Continuous Integration (CI)** stands for Continuous Integration, which is the practice of merging all developers’ working copies to a shared mainline several times a day.

- **REST** is software architectural style that was created to guide the design and development of the architecture for the World Wide Web.

- **Data Model** is an abstract model that organizes data description, data semantics, and consistency constraints of data. The data model emphasizes on what data is needed and how it should be organized instead of what operations will be performed on data.

## Preparation Materials

- **sql vs nosql (Video)**

  - SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.

  - SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to..

  - SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.

  - SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.

  - SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.

  - SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb.

- **nosql vs sql**

SQL databases are primarily called as Relational Databases (RDBMS).

- SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores.

- SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.

- For scalability: In most typical situations, SQL databases are vertically scalable.

***SQL Database Examples***

* MySQL Community Edition.

* MS-SQL Server Express Edition.

* Oracle Express Edition

***NoSQL Database Examples***

* MongoDB.

* CouchDB.

* Redis.

***nosql modeling techniques***

  NoSQL databases are compared by various non-functional criteria, such as scalability, performance, and consistency. This aspect of NoSQL is well-studied both in practice and theory because specific non-functional properties are often the main justification for NoSQL usage and fundamental results on distributed systems like the CAP theorem apply well to NoSQL systems.
