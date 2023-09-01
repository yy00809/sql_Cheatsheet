# sql_Instructions
1.SELECT /SELECT DISTINCT

2.COUNT

3.WHERE

4.ORDER BY

5.LIMIT

6.BTWEEN ... AND ...

7.IN

8.LIKE/ILIKE

9.GROUP BY

10.HAVING

11.AS

12.INNER JOIN

13.FULL JOIN

14.LEFT JOIN

15.RIGHT JOIN

16.UNION

17.TIMESTAMPS and EXTRACT (EXTRACT (YEAR FROM date_col))

18.Subquery allows you to use two select commands

19.EXISTIS() function to check if any rows are retruned with the subquery

20.CREATE TABLE 

21.INSERT

22.UPDATE DELETE

23.ALTER

24.DROP

25.CHECK

26.
CASE
SELECT
CASE rentqal_rate
  WHEN 0.99 THEN 1
  ELSE 0
END ) AS number_of_bargains
FROM film

27.COALESCE function accepts an unlimited nummber of arguments. It returns the first argument that is not null. If all arguments are null, the function will return null. Useful when querying a table that contains null values and substituting it with another value.

SELECT item,(price - COALESCE(discount,0)) AS final FROM table  COLASESCIE replace the nulls in discount with 0.

28. CAST operator let's you convert from one data type into another
SELECT CAST(colum AS INTEGER) column have string of '1'
OR '5'::INTEGER in POSTGREsql

29.NULLIF
takes in 2 inputs and returns null if both are equal, otherwise it returns the first argument.
This is usedful where a null would cause an error. TO check if the val1 is equal to 0;

30. saving a repeatedly used query as a view in PostgreSQL
CREATE VIEW name AS the query.
AFTER, you can just use the name to refer to the query instead of writing the whole query again.

31.import csv.file in pgadmin.
Fisrt, create a table with the same columns as in the csv.file
Then, press import after right click on the table in the schema 
