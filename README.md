## PostgreSQL Queries - Patika.dev ASP.NET Core Week 6 Assignment
This repository contains SQL queries related to the PostgreSQL database as part of the Week 6 assignment for the Patika.dev ASP.NET Core course. The queries are designed to perform various operations on the film and customer tables of a sample database.

## Queries Overview
# 1. Retrieve title and description columns from the film table
```sql
Copy code
SELECT title, description FROM film; 
``` 


This query selects and displays the title and description columns from all rows in the film table.

# 2. Retrieve all columns from the film table where the length is greater than 60 and less than 75
```sql
Copy code
SELECT * FROM film WHERE length > 60 AND length < 75;``` 
This query returns all columns from the film table for rows where the length is between 60 and 75.

# 3. Retrieve all columns from the film table where the rental_rate is 0.99 and the replacement_cost is either 12.99 or 28.99
```sql
Copy code
SELECT * FROM film WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);``` 

This query filters the film table to display rows where the rental_rate is 0.99 and the replacement_cost is either 12.99 or 28.99.

# 4. Retrieve the last_name of customers with the first name 'Mary'
```sql
Copy code
SELECT last_name FROM customer WHERE first_name = 'Mary';``` 

This query selects and displays the last_name of customers from the customer table where the first_name is 'Mary'.

# 5. Retrieve all columns from the film table where the length is not greater than 50 and the rental_rate is not 2.99 or 4.99
```sql
Copy code
SELECT * FROM film WHERE length < 50 AND NOT(rental_rate = 2.99 OR rental_rate = 4.99);``` 

This query returns all columns from the film table for rows where the length is less than 50 and the rental_rate is neither 2.99 nor 4.99.

Getting Started
To run these queries, you need access to a PostgreSQL database with the appropriate tables (film and customer). You can execute these queries using any PostgreSQL client such as pgAdmin, psql, or DBeaver.

License
This project is licensed under the MIT License.
