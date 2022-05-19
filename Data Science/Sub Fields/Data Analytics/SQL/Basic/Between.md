The `BETWEEN` operator selects values within a given range. The values can be numbers, text, or dates.

The `BETWEEN` operator is inclusive: begin and end values are included.

# BETWEEN  Syntax

```SQL
SELECT _column_name(s)_  
FROM _table_name_  
WHERE _column_name_ BETWEEN _value1_ AND _value2_);
```

# BETWEEN Operator Examples

The following SQL statement selects all products with a price between 10 and 20:

```SQL
SELECT * FROM Products  
WHERE Price BETWEEN 10 AND 20;
```

To display the products outside the range of the previous example, use `NOT BETWEEN`:

```SQL
SELECT * FROM Products  
WHERE Price NOT BETWEEN 10 AND 20;
```

The following SQL statement selects all products with a price between 10 and 20. In addition; do not show products with a CategoryID of 1,2, or 3:

```SQL
SELECT * FROM Products  
WHERE Price BETWEEN 10 AND 20  
AND CategoryID NOT IN (1,2,3);
```

The following SQL statement selects all products with a ProductName between Carnarvon Tigers and Mozzarella di Giovanni:

```SQL
SELECT * FROM Products  
WHERE ProductName BETWEEN 'Carnarvon Tigers' AND 'Mozzarella di Giovanni'  
ORDER BY ProductName;
```