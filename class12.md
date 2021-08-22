# Mongo and Mongoose

## differences between SQL and NoSQL

| SQL                          | NOSQL                                                  |
| -----------------------------| -------------------------------------------------------|
|Relational Databases (RDBMS)       | non-relational or distributed database.           |
|databases are table based databases|databases are document based                       |
| databases have predefined schema  |databases have dynamic schema for unstructured data|
| databases are vertically scalable | databases are horizontally scalable               |

**For high transactional based application: SQL databases are best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data. While you can use NoSQL for transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications.**

## SQL Database Examples

* **MySQL Community Edition**

**MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js.**

## NOSQL Database Examples

* **MongoDB**

**Mongodb is one of the most popular document based NoSQL database as it stores data in JSON like documents. It is non-relational database with dynamic schema. It has been developed by the founders of DoubleClick, written in C++ and is currently being used by some big companies like The New York Times, Craigslist, MTV Networks. The following are some of MongoDB benefits and strengths:**

## What is SQL and what's it got to do with Microsoft Access

**SQL (pronounced "ess-que-el")** _stands for Structured Query Language. SQL is used to communicate with a database. According to ANSI (American National Standards Institute), it is the standard language for relational database management systems._

**SQL statements** _are used to perform tasks such as update data on a database, or retrieve data from a database. Some common relational database management systems that use SQL are: Oracle, Sybase, Microsoft SQL Server, Microsoft Access, Ingres, etc._

_Although most database systems use SQL, most of them also have their own additional proprietary extensions that are usually only used on their system. However, the standard SQL commands such as "Select", "Insert", "Update", "Delete", "Create", and "Drop" can be used to accomplish almost everything that one needs to do with a database._

## Relational Database (RDBMS)

**A relational database is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables. In a relational database, each row in the table is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points.**

## relational databases structure

**The relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures. This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure. For example, renaming a database file does not rename the tables stored within it.**

_The distinction between logical and physical also applies to database operations, which are clearly defined actions that enable applications to manipulate the data and structures of the database. Logical operations allow an application to specify the content it needs, and physical operations determine how that data should be accessed and then carries out the task._

## database schema

**A database schema** _represents the logical configuration of all or part of a relational database. It can exist both as a visual representation and as a set of formulas known as integrity constraints that govern a database. These formulas are expressed in a data definition language, such as SQL. As part of a data dictionary, a database schema indicates how the entities that make up the database relate to one another, including tables, views, stored procedures, and more._

![d](https://d2slcw3kip6qmk.cloudfront.net/marketing/pages/chart/seo/database/discovery/logical-physical-schema.svg)
__________________________________________________________________________________________________________________________________________

## NoSQL database

 **refer to any non-relational database. Some say the term “NoSQL” stands for “non SQL” while others say it stands for “not only SQL.” Either way, most agree that NoSQL databases are databases that store data in a format other than relational tables.**

## disadvantage  NoSQL database


* **NoSQL databases don’t have the reliability functions which Relational Databases have (basically don’t support ACID).**
**This also means that NoSQL databases offer consistency in performance and scalability.**
* **In order to support ACID developers will have to implement their own code, making their systems more complex.**
**This may reduce the number of safe applications that commit transactions, for example bank systems.**
* **NoSQL is not compatible (at all) with SQL.**
**Some NoSQL management systems do use a Structured Query Language.**
**This means that you will need a manual query language, making things slower and more complex.**
* **NoSQL are very new compared to Relational Databases, which means that are far less stable and may have a lot less functionalities.**