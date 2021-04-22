
.. contents::
   :local:
   :depth: 3
   
SQL commands are mainly categorized into four categories as:(database language)
===============================================================================

DDL(Data Definition Language) :
--------------------

It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. 

Ex: 

CREATE ,

DROP ,

ALTER,

TRUNCATE,

COMMENT,

RENAME

DQL (Data Query Language) :
--------------------

DQL statements are used for performing queries on the data within schema objects.

Ex : SELECT


DML(Data Manipulation Language):
--------------------

The SQL commands that deals with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. 
Examples of DML: 

INSERT 

UPDATE

DELETE


DCL(Data Control Language):
--------------------

DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions and other controls of the database system. 

Examples of DCL commands: 

GRANT-gives user’s access privileges to the database.

REVOKE-withdraw user’s access privileges given by using the GRANT command.

TCL(transaction Control Language):
--------------------

TCL commands deal with the transaction within the database. 

Examples of TCL commands: 

COMMIT– commits a Transaction.

ROLLBACK– rollbacks a transaction in case of any error occurs.

SAVEPOINT–sets a savepoint within a transaction.

SET TRANSACTION–specify characteristics for the transaction.



What is normalization?
===============================================================================

Normalization is used to minimize redundancy and dependency by organizing fields and table of a database. Normalization breaks the table into small partitions
and then link them using different relationships so that it will avoid the chances of redundancy.


First Normal Form (1NF):
--------------------

This should remove all the duplicate columns from the table. Creation of tables for the related data and identification of unique columns.

Second Normal Form (2NF):
--------------------

Meeting all requirements of the first normal form. Placing the subsets of data in separate tables and Creation of relationships between the tables using primary keys.

Third Normal Form (3NF):
--------------------

This should meet all requirements of 2NF. Removing the columns which are not dependent on primary key constraints.

Fourth Normal Form (4NF):
--------------------

Meeting all the requirements of third normal form and it should not have multi- valued dependencies.
