The `WHERE` clause can be combined with `AND`, `OR`, and `NOT` operators.

The `AND` and `OR` operators are used to filter records based on more than one condition:

-   The `AND` operator displays a record if all the conditions separated by `AND` are TRUE.
-   The `OR` operator displays a record if any of the conditions separated by `OR` is TRUE.

The `NOT` operator displays a record if the condition(s) is NOT TRUE.

## AND Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE _condition1_ AND _condition2_ AND _condition3 ..._;
```

## OR Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE _condition1_ OR _condition2_ OR _condition3 ..._;
```

## Combining OR and AND Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE (_condition1_ OR _condition2_) AND _condition3 ..._;
```

## NOT Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE NOT _condition_;
```

## Combining OR and AND NOT Syntax

```SQL
SELECT _column1_, _column2, ..._  
FROM _table_name_  
WHERE (_condition1_ OR _condition2_) AND NOT _condition3 ..._;
```
