The `LIKE` operator is used in a `WHERE` clause to search for a specified pattern in a column.

There are two wildcards often used in conjunction with the `LIKE` operator:

-    The percent sign (`%`) represents **zero**, **one**, or **multiple** characters
-    The underscore sign (`_`) represents one, single character

```ad-hint
The percent sign and the underscore can also be used in combinations!
```

## Syntax


```SQL
SELECT _column1, column2, ..._  
FROM _table_name_  
WHERE _columnN_ LIKE _pattern_;
```

```ad-tip
**Tip:** You can also combine any number of conditions using `AND` or `OR` operators.
```

## Examples

<table class="ws-table-all notranslate">
  <tbody><tr>
    <th>LIKE Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE 'a%'</td>
    <td>Finds any values that start with "a"</td>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE '%a'</td>
    <td>Finds any values that end with "a"</td>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE '%or%'</td>
    <td>Finds any values that have "or" in any position</td>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE '_r%'</td>
    <td>Finds any values that have "r" in the second position</td>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE 'a_%'</td>
    <td>Finds any values that start with "a" and are at least 2 characters in length</td>
  </tr>
  <tr>
    <td>WHERE CustomerName LIKE 'a__%'</td>
    <td>Finds any values that start with "a" and are at least 3 characters in length</td>
  </tr>
  <tr>
    <td>WHERE ContactName LIKE 'a%o'</td>
    <td>Finds any values that start with "a" and ends with "o"</td>
  </tr>
</tbody></table>
