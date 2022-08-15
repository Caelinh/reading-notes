## Queries with constraints
| Operator  |  Condition | SQL Example  |
|---|---|---|
| =, !=, < <=, >, >=  |  	Standard numerical operators | col_name != 4  |
|  BETWEEN … AND … | Number is within range of two values (inclusive)  |  col_name BETWEEN 1.5 AND 10.5 |
|  NOT BETWEEN … AND … | Number is not within range of two values (inclusive)  | col_name NOT BETWEEN 1 AND 10  |
|  IN (…) | Number exists in a list  | 	col_name IN (2, 4, 6)  |
| NOT IN (…)  |  Number does not exist in a list |  col_name NOT IN (1, 3, 5) |

![SQL 1](https://user-images.githubusercontent.com/106052558/184562811-39a12d14-e7f2-4fbf-b0da-76060372d05d.png)
![SQL 2](https://user-images.githubusercontent.com/106052558/184562822-f369331e-25c6-4555-9305-5a115f9e1d6c.png)


## Queries with constraints (Pt. 2) 

| Operator  |  Condition | SQL Example  |
|---|---|---|
|=|	Case sensitive exact string comparison (notice the single equals)	|col_name = "abc" |
|!= or <>|	Case sensitive exact string inequality comparison	|col_name != "abcd" |
|LIKE|	Case insensitive exact string comparison|	col_name LIKE "ABC" |
|NOT LIKE|	Case insensitive exact string inequality comparison	|col_name NOT LIKE "ABCD" |
|%|	Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)	|col_name LIKE "%AT%"
(matches "AT", "ATTIC", "CAT" or even "BATS") |
|_ |	Used anywhere in a string to match a single character (only with LIKE or NOT LIKE)	|col_name LIKE "AN_"
(matches "AND", but not "AN") |
|IN (…) |	String exists in a list	| col_name IN ("A", "B", "C") |
|NOT IN (…) |	String does not exist in a list	|col_name NOT IN ("D", "E", "F") |

![SQL 3](https://user-images.githubusercontent.com/106052558/184562832-fba01513-e940-491f-81b8-4b0dc9ffa673.png)


## Filtering and sorting Query results 

 SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.  
 **Disctinct**
````
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
````
**Order By**  
````
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
````

**LIMIT and OFFSET**  
````
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
````
![sql 4](https://user-images.githubusercontent.com/106052558/184562838-66c6de81-79f5-4b47-8fc5-b193f61576a2.png)
![sql 6](https://user-images.githubusercontent.com/106052558/184562842-0ecc1c58-e2de-4292-a623-aceae9d26e20.png)


## Multi-table queries with JOINs
**Using the JOIN clause in a query, we can combine row data across two separate tables using this unique key. The first of the joins that we will introduce is the INNER JOIN.**  
````
SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
````  
The INNER JOIN is a process that matches rows from the first table and the second table which have the same key (as defined by the ON constraint) to create a result row with the combined columns from both tables. After the tables are joined, the other clauses we learned previously are then applied.

![sql 7](https://user-images.githubusercontent.com/106052558/184562849-451bca3e-60bd-441d-bbb7-5dd919c429dc.png)

## Inserting data

````
Insert statement with values for all columns
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
````  

![sql 14](https://user-images.githubusercontent.com/106052558/184563443-4b572d53-e9c3-4266-a850-5e9e5b491857.png)

## Updating Rows

````
UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;
````
![sql 15](https://user-images.githubusercontent.com/106052558/184563488-ed86983f-ac53-4df5-beec-748ec3c68ce3.png)

## Deleting rows

````
DELETE FROM mytable
WHERE condition;
````  

![sql 16](https://user-images.githubusercontent.com/106052558/184563620-676450b2-0db6-4ff9-91bd-b3333916113a.png)  

##  Creating tables

````
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
````
**Example table**  
````
CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER, 
    length_minutes INTEGER
);
````

![sql 17](https://user-images.githubusercontent.com/106052558/184563712-c8229013-41aa-4717-8f0b-7bdfba679784.png)
 
 ## Altering Tables  
 
 ### Adding Columns
 
 ````
 ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
````

### Removing Columns  

````
 ALTER TABLE mytable
DROP column_to_be_deleted;
````

### Renaming Columns

````
ALTER TABLE mytable
RENAME TO new_table_name;
````


![sql 18](https://user-images.githubusercontent.com/106052558/184563839-8411c41a-56b7-4676-bfc5-1b97f55ea11a.png)  

## Dropping tables
````
DROP TABLE IF EXISTS mytable;
````
![sql 19](https://user-images.githubusercontent.com/106052558/184563880-756d5b94-c125-49b2-9f71-2419becd7385.png)



