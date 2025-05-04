```sql
-- IS NULL Keyword
SELECT *
FROM customers
WHERE phone IS NULL
```

    This SQL query selects all columns from the `customers` table where the `phone` column is NULL. The `IS NULL` keyword is used to filter records that have no value in the specified column.

```sql
-- IS NULL Keyword
SELECT *
FROM orders
WHERE shipper_id IS NULL
```

    This SQL query selects all columns from the `orders` table where the `shipper_id` column is NULL. The `IS NULL` keyword is used to filter records that have no value in the specified column.
