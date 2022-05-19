The `WHERE` clause is used to filter records.

It is used to extract only those records that fulfill a specified condition.

## WHERE Syntax


```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE _condition_;
```

```ad-hint
**Note:** The `WHERE` clause is not only used in `SELECT` statements, it is also used in `UPDATE`, `DELETE`, etc.!
```

## Text Fields vs. Numeric Fields

SQL requires single quotes around text values (most database systems will also allow double quotes).

```SQL
SELECT * FROM Customers  
WHERE Country='Mexico';
```

However, numeric fields should not be enclosed in quotes

```SQL
SELECT * FROM Customers  
WHERE CustomerID=1;
```

## Operators

<table class="ws-table-all notranslate">
  <tbody><tr>
    <th style="width:20%">Operator</th>
    <th style="width:70%">Description</th>
  </tr>
  <tr>
    <td>=</td>
    <td>Equal</td>
    <td><a target="_blank" class="w3-btn btnsmall" h
  </tr>
  <tr>
    <td>&gt;</td>
    <td>Greater than</td>
  </tr>
  <tr>
    <td>&lt;</td>
    <td>Less than</td>
  </tr>
  <tr>
    <td>&gt;=</td>
    <td>Greater than or equal</td>
  </tr>
  <tr>
    <td>&lt;=</td>
    <td>Less than or equal</td>
  </tr>
  <tr>
    <td>&lt;&gt;</td>
    <td>Not equal. <b>Note:</b> In some versions of SQL this operator may be written as !=</td>
  </tr>
  <tr>
    <td>BETWEEN</td>
    <td>Between a certain range</td>
  </tr>
  <tr>
    <td>LIKE</td>
    <td>Search for a pattern</td>
  </tr>
  <tr>
    <td>IN</td>
    <td>To specify multiple possible values for a column</td>
  </tr>
</tbody></table>

The following SQL statement selects the "CustomerName" and "City" columns from the "Customers" table:

```SQL
SELECT CustomerName, City
FROM Customers;
```

The following SQL statement selects all the columns from the "Customers" table:

```SQL
SELECT * FROM Customers;```
