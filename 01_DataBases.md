/***************SQL CHEAT SHEET********/
-------------------------------------------
/***************1. SQL Basic Commands********/
-------------------------------------------
// to create a database
CREATE DATABASE myDB;

// To use the databse
USE myDB;

// to delete the database
DROP DATABASE myDB;
 
// to alter the databse
ALTER DATABASE myDB READ ONLY = 1/0;
------------------------------------------
/***************2. SQL Create,Select,Reanme,Alter Table********/
-------------------------------------------
1)
create table emplyoees(
    emp_id INT,
    first_name VARCHAR(15),
    last_name VARCHAR(15),
    hourly_pay DECIMAL(5,2),
    age INT(2),
)

2)
SELECT * FROM emplyoees;

3)  
Rename table emplyoees to workers;

4)
ALTER TABLE emplyoees
RENAME COLUMN age to joining_date;

5)
ALTER TABLE emplyoees
MODIFY COLUMN email VARCHAR(100);
------------------------------------------
/***************3. SQL Change the position of Column********/
-------------------------------------------
1) Alter table Workers
Modify age INT(2)
AFTER last_name;

SELECT * FROM workers;

