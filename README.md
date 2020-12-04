- [Basic Installation (Ubuntu 20.04)](#basic-installation-ubuntu-2004)
- [1. What is Northwind?](#1-what-is-northwind)
- [2. SQL command classes](#2-sql-command-classes)
- [3. Accessing PostgreSQL with psql command line client](#3-accessing-postgresql-with-psql-command-line-client)
- [4. DDL](#4-ddl)

# Basic Installation (Ubuntu 20.04)

    # apt install postgresql postgresql-contrib

# 1. What is Northwind?

Northwhind it's a database sample that was made available by Microsoft.

[PostgreSQL's example.](#https://github.com/pthom/northwind_psql)

# 2. SQL command classes

**SQL (Structured Query Language)**  
├── **DCL (Data Control Language)**  
│   ├── Grant  
│   └── Revoke  
├── **DDL (Data Definition Language)**  
│   ├── Alter  
│   ├── Create  
│   ├── Drop  
│   ├── Rename  
│   └── Truncate  
├── **DML (Data Manipulation Language)**  
│   ├── Delete  
│   ├── Insert  
│   ├── Select  
│   └── Update  
├── **TCL (Transaction Control Language)**  
│   ├── Start Transaction  
│   ├── Commit  
│   └── Rollback 

# 3. Accessing PostgreSQL with psql command line client

3.1. Accessing psql with postgres user
    
    
    $ psql -U postgres
    

3.2. If you need some help

    postgres=# help

3.3. Command summary

    postgres=# \h