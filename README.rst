
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



