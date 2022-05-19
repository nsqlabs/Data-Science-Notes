The `LIMIT` statement is used to limit the number of rows that are retrieved from a query.

The following SQL statement selects the "CustomerName" and "City" columns from the 10 first entries in the "Customers" table:

```SQL
SELECT CustomerName, City
FROM Customers
LIMIT 10;
```

The following SQL statement selects all the columns rom the 10 first entries in the "Customers" table:

```SQL
SELECT * FROM Customers
LIMIT 10;
```
