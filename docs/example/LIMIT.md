```sql
-- LIMIT Keyword
SELECT *
FROM customers
LIMIT 3;

```

```sql
-- LIMIT Keyword
SELECT *
FROM customers
LIMIT 6,3;

```

This example demonstrates how to use the `LIMIT` keyword to restrict the number of rows returned by a query. The first query selects all customers but limits the result set to 3 rows. The second query uses the `LIMIT` keyword with two arguments, which specifies an offset and a row count. In this case, it skips the first 6 rows and returns the next 3 rows from the result set.

```sql
-- LIMIT Keyword
SELECT *
FROM customers
ORDER BY points DESC
LIMIT 3;

```

This example demonstrates how to use the `LIMIT` keyword in conjunction with the `ORDER BY` clause to restrict the number of rows returned by a query. The query selects all customers, orders them by their points in descending order, and limits the result set to 3 rows. This will return the top 3 customers with the highest points.
