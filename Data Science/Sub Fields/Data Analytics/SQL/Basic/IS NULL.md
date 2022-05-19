A field with a `NULL` value is a field with no value.

If a field in a table is optional, it is possible to insert a new record or update a record without adding a value to this field. Then, the field will be saved with a `NULL` value.

## How to Test for NULL Values?

It is not possible to test for NULL values with comparison operators, such as `=`, `<`, or `<>`.

We will have to use the `IS NULL` and `IS NOT NULL` operators instead.

# IS NULL Syntax

```SQL
SELECT _column_names  
_FROM _table_name_  
WHERE _column_name_ IS NULL;
```

# IS NOT NULL Syntax

```SQL
SELECT _column_names  
_FROM _table_name_  
WHERE _column_name_ IS NOT NULL;
```

# IS NULL Operator Examples

The following SQL lists all customers with a NULL value in the "Address" field:

```SQL
SELECT CustomerName, ContactName, Address  
FROM Customers  
WHERE Address IS NULL;
```

# IS NOT NULL Operator Examples

The following SQL lists all customers with a value in the "Address" field:

```SQL
SELECT CustomerName, ContactName, Address  
FROM Customers  
WHERE Address IS NOT NULL;
```