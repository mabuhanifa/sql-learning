```sql
-- Between Keyword
SELECT *
FROM customers
WHERE points >= 1000 AND points <=3000;
```

```sql
-- Between Keyword
SELECT *
FROM customers
WHERE points BETWEEN 1000 AND 3000;
```

This example shows how to use the BETWEEN keyword to filter results based on a range of values. The first query uses the AND operator to specify the range, while the second query uses the BETWEEN keyword for a more concise syntax. Both queries will return the same result set, which includes all customers with points between 1000 and 3000, inclusive.

```sql
-- Between Keyword
SELECT *
FROM customers
WHERE birth_date BETWEEN "1990-01-01" AND "2000-01-01";
```

This example shows how to use the BETWEEN keyword to filter results based on a range of dates. The query will return all customers whose birth date falls between January 1, 1990, and January 1, 2000, inclusive.
