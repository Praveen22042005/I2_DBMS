# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```
CREATE TABLE students(rollno INT,name VARCHAR(100),age INT,address VARCHAR(100),phoneno VARCHAR(15));
```

### OUTPUT:
![image](https://github.com/Praveen22042005/I2_DBMS/assets/112475766/7521c450-3a93-4eaf-aa3c-5bb216c6b620)


### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```
INSERT INTO students(rollno, name, age, address, phoneno) VALUES (1, 'John', 20, 'CHENNAI', '9153657854');
INSERT INTO students(rollno, name, age, address, phoneno) VALUES (2, 'SMITH', 25, 'TRICHY', '9746441548');
```

### OUTPUT:
![image](https://github.com/Praveen22042005/I2_DBMS/assets/112475766/a1e972a5-0ba6-4650-b60e-4ce6557926e8)


### 3) Drop the student table
 
### SQL QUERY: 
```
ALTER TABLE students RENAME TO mystudent;
```


### OUTPUT:
![image](https://github.com/Praveen22042005/I2_DBMS/assets/112475766/68f20d2e-cbf6-4dbc-ac2b-c98cb37884d2)


### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE mystudent;
```


### OUTPUT:
![image](https://github.com/Praveen22042005/I2_DBMS/assets/112475766/3e111798-2d54-43af-90fb-f318444efd2f)



### 5) Rename the student table to mystudent

### SQL QUERY: 
```
DROP TABLE students;
```


### OUTPUT:
![image](https://github.com/Praveen22042005/I2_DBMS/assets/112475766/5150d997-a276-447a-a443-95115a0c2663)

