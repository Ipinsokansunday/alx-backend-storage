# Project: 0x00-MySQL_Advanced
This project focuses on advanced MySQL concepts and operations. It is part of the ALX Backend Storage curriculum, where you will deepen your understanding of database management and SQL scripting.

Requirements
MySQL Version: 5.7 (version 5.7.30)
Operating System: Ubuntu 18.04 LTS
General Rules:
All SQL queries must be preceded by a comment explaining their purpose.
All SQL keywords should be in uppercase (e.g., SELECT, WHERE).
Each SQL file should end with a new line.
Learning Objectives
By completing this project, you will learn:

How to create and manage MySQL databases and tables.
How to enforce data integrity and avoid bugs by defining constraints.
How to manipulate data using advanced SQL queries.
How to perform operations on data and tables within MySQL.
Project Structure
0-uniq_users.sql: This script creates a table named users with attributes id, email, and name. The email field is unique to enforce business rules and avoid duplicates.
Usage
To execute the SQL scripts in this project:

Start MySQL:

bash
Copy code
service mysql start
Execute a script:

bash
Copy code
cat 0-uniq_users.sql | mysql -uroot -p
Examples
Inserting data into the users table:

sql
Copy code
INSERT INTO users (email, name) VALUES ("bob@dylan.com", "Bob");
Attempting to insert a duplicate email:

sql
Copy code
INSERT INTO users (email, name) VALUES ("bob@dylan.com", "Jean");
-- This will result in an error due to the unique constraint on the email field.
Author
This project was completed as part of the ALX Backend Storage program.
