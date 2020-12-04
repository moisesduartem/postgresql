- [Basic Installation (Ubuntu 20.04)](#basic-installation-ubuntu-2004)
- [1. What is Northwind?](#1-what-is-northwind)
- [2. SQL command classes](#2-sql-command-classes)
- [3. Command line client (psql) basic usage](#3-command-line-client-psql-basic-usage)
- [4. DDL](#4-ddl)

# Basic Installation (Ubuntu 20.04)

    # apt install postgresql postgresql-contrib

# 1. What is Northwind?

Northwhind it's a database sample that was made available by Microsoft.

[PostgreSQL's example.](https://github.com/pthom/northwind_psql)

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

# 3. Command line client (psql) basic usage

3.1. Checking version

    $ psql --version

3.2. Command list before access psql

    $ psql --help

3.3. Accessing psql with postgres user without password    
    
    $ psql -U postgres
    
3.4. Defining password

    postgres=# \password

3.5. Show informations about some sql command

    Example with "create role": 
    postgres=# \h create role

3.5. Show informations about some psql command

    Example with "\password": 
    postgres=# \? \password

3.6. List databases

    postgres=# \l

3.7. List roles (users)

    postgres=# \du

3.8. Change database passing the name

    postgres=# \c other_database

3.8. List the database relationships

    postgres=# \dS

3.9. If you need some help

    postgres=# help

3.10. psql intern command summary

    postgres=# \h

3.11. Show hba file path

    postgres=# show hba_file;

# 4. DDL

4.1. Creating database
    
    create database northwhind

4.2. Dropping database
    
    drop database northwhind