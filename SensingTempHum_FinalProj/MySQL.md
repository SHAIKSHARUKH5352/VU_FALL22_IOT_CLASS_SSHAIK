## What is MySQL?

MySQL, pronounced either "My S-Q-L" or "My Sequel," is an open source relational database management system. It is based on the structure query language (SQL), which is used for adding, removing, and modifying information in the database. Standard SQL commands, such as ADD, DROP, INSERT, and UPDATE can be used with MySQL.

## MySQL Installation

Install MySQL from the link ''' https://dev.mysql.com/downloads/installer/ '''

You have to have Oracle account for MySQL installation.

## Database Tables for the project
```
create database temp_hum;
use temp_hum;
create table temp( tmp FLOAT, date_recorded DATE, time_recorded TIME);
create table humidity( hum NOT FLOAT, date_rec DATE, time_rec TIME);

```





