# SQL for Data Science

# Objective: 

Introduction to databases and rational concepts by create a database instance on the the could. Explode the basic SQL for Data Science. 

# Tool Used:
Used Jupyter to code and connecting IBM DB2 Warehouse on Cloud Database and run SQL Queries. Load datasets into three tables in a DB2 database. 

# Datasets

Census Data - Selected socioeconomic indicators in Chicago, 2008-2012
https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2 

Chicago Public Schools - Project Report Card (2011-2012)
https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t  

Crimes - 2001 to Present 
https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2 


# Store datasets in database table

Load the SQL extension %load_ext sql  and enter the connection string on your DB2 on cloud database.  

# Five basic SQL commands  

1. INSERT data into the table
2. SELECT data from the table
3. UPDATE data from the table
4. DELETE data from the table

Crate Table INSTRUCTOR 
(ins_id INTEGER PRIMARY KEY NOT NULL,
lastname VARCHAR(15) NOT NULL,
firstname VARCHAR(15) NOT NULL,
city VARCHAR(15),
country CHAR(2)
);

INSERT single row for Johnny Apple 
INSERT into INSTRUCTOR 
  (ins_id, lastname, firstname, city, country)
  VALUES 
  (1, "Apple", "Johnny", "Los Angeles", "US")

SELECT all rows in the table 
SELECT * FROM INSTRUCTOR 

Change the city name from US to UK
UPDATE INSTRUCTOR SET city='UK" WHERE ins_id=1

# To Retrieve data by a SELECT statement and adding the WHERE clause to set a condition search

Restricting the result set by using the comparison operator in the WHERE clause and always include a condition expression (Predicate). 

List of the basic comparison operators 
1. Equal to =
2. Greater than >
3. Lesser than <
4. Greater than or equal to >=
5. Less than or equal to <=
6. Not equal to <>

List of the SQL Logical Operator 
1. All 
2. And
3. Any
4. Between 
5. Exists 
6. In 
7. Like 
8. Not 
9. Or 
10. Some 


