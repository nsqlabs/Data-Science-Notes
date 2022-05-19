The `ORDER BY` keyword is used to sort the result-set in ascending or descending order.

The `ORDER BY` keyword sorts the records in ascending order by default. To sort the records in descending order, use the `DESC` keyword..

# Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
ORDER BY _column1, column2, ..._ ASC|DESC;
```

# Examples

The following SQL statement selects all customers from the "Customers" table, sorted by the "Country" column:

```SQL
SELECT * FROM Customers  
ORDER BY Country;
```

The following SQL statement selects all customers from the "Customers" table, sorted DESCENDING by the "Country" column:

```SQL
SELECT * FROM Customers  
ORDER BY Country DESC;
```

The following SQL statement selects all customers from the "Customers" table, sorted by the "Country" and the "CustomerName" column. This means that it orders by Country, but if some rows have the same Country, it orders them by CustomerName:

```SQL
SELECT * FROM Customers  
ORDER BY Country, CustomerName;
```