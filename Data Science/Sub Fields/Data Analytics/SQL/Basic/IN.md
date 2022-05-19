The `IN` operator allows you to specify multiple values in a `WHERE` clause.

The `IN` operator is a shorthand for multiple `OR` conditions.

# IN  Syntax

```SQL
SELECT _column_name(s)_  
FROM _table_name_  
WHERE _column_name_ IN (_value1_, _value2_, ...);
```
or:

```SQL
SELECT _column_name(s)_  
FROM _table_name_  
WHERE _column_name_ IN (_SELECT STATEMENT_);
```

# IN Operator Examples

The following SQL statement selects all customers that are located in "Germany", "France" or "UK":

```SQL
SELECT * FROM Customers  
WHERE Country IN ('Germany', 'France', 'UK');
```

The following SQL statement selects all customers that are NOT located in "Germany", "France" or "UK":

```SQL
SELECT * FROM Customers  
WHERE Country NOT IN ('Germany', 'France', 'UK');
```

The following SQL statement selects all customers that are from the same countries as the suppliers:

```SQL
SELECT * FROM Customers  
WHERE Country IN (SELECT Country FROM Suppliers);
```