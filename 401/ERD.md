 # ERD

## Schema
 - [What is a database schema?](https://www.lucidchart.com/pages/database-diagram/database-schema)
    >The term "database schema" can refer to a visual representation of a database, a set of rules that govern a database, or to the entire set of objects belonging to a particular user. Read on to find out more about database schemas and how they are used.

 - [Why do we use them?](https://www.postgresql.org/docs/8.1/ddl-schemas.html#:~:text=There%20are%20several%20reasons%20why,to%20make%20them%20more%20manageable.)
    > There are several reasons why one might want to use schemas: To allow many users to use one database without interfering with each other. To organize database objects into logical groups to make them more manageable.

 - [What do they look like?](https://www.lucidchart.com/pages/database-diagram/database-schema)
    > A database schema represents the logical configuration of all or part of a relational database. It can exist both as a visual representation and as a set of formulas known as integrity constraints that govern a database. These formulas are expressed in a data definition language, such as SQL. As part of a data dictionary, a database schema indicates how the entities that make up the database relate to one another, including tables, views, stored procedures, and more.

## Database Keys

 - [What is a Primary Key?](https://www.w3schools.com/sql/sql_primarykey.ASP#:~:text=The%20PRIMARY%20KEY%20constraint%20uniquely,or%20multiple%20columns%20(fields).)
    > The PRIMARY KEY constraint uniquely identifies each record in a table. Primary keys must contain UNIQUE values, and cannot contain NULL values. A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).

 - [What is a Foreign Key?](https://www.w3schools.com/sql/sql_foreignkey.asp#:~:text=A%20FOREIGN%20KEY%20is%20a,PRIMARY%20KEY%20in%20another%20table.)
    > A FOREIGN KEY is a key used to link two tables together. A FOREIGN KEY is a field (or collection of fields) in one table that refers to the PRIMARY KEY in another table.

 - [What is a Composite Key?](https://en.wikipedia.org/wiki/Compound_key#:~:text=In%20database%20design%2C%20a%20composite,key%20in%20its%20own%20right.)
    > In database design, a composite key is a candidate key that consists of two or more attributes (table columns) that together uniquely identify an entity occurrence (table row). A compound key is a composite key for which each attribute that makes up the key is a simple (foreign) key in its own right.


## Relationships in a relational database

 - [What is a 1:1 relationship?](https://bit.ly/3bCsZnX)
    > A one-to-one (1:1) relationship means that each record in Table A relates to one, and only one, record in Table B, and each record in Table B relates to one, and only one, record in Table A.

 - [What is a Many:Many relationship?](https://fmhelp.filemaker.com/help/18/fmp/en/FMP_Help/many-to-many-relationships.html#:~:text=A%20many%2Dto%2Dmany%20relationship,multiple%20records%20in%20another%20table.&text=Relational%20database%20systems%20usually%20don,of%20keeping%20track%20of%20invoices.)
    > A many-to-many relationship occurs when multiple records in a table are associated with multiple records in another table. ... Relational database systems usually don't allow you to implement a direct many-to-many relationship between two tables.

 - [How about a 1: Many or a Many:1?](https://fmhelp.filemaker.com/help/18/fmp/en/index.html#page/FMP_Help/one-to-many-relationships.html)
    > In a one-to-many relationship, one record in a table can be associated with one or more records in another table. 