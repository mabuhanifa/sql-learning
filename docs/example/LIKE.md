```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE last_name LIKE 'brush%'
```

    This example demonstrates how to use the `LIKE` keyword to filter results based on a pattern. The query selects all customers whose last name starts with "brush". The `%` wildcard character represents zero or more characters, so this will match any last name that begins with "brush", such as "brush", "brushing", or "brushed".

```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE last_name LIKE '%y'
```

    This example demonstrates how to use the `LIKE` keyword to filter results based on a pattern. The query selects all customers whose last name ends with "y". The `%` wildcard character represents zero or more characters, so this will match any last name that ends with "y", such as "Smithy", "Jonesy", or "Miller".

```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE last_name LIKE '_____y'
```

    This example demonstrates how to use the `LIKE` keyword to filter results based on a pattern. The query selects all customers whose last name has exactly five characters and ends with "y". The `_` wildcard character represents a single character, so this will match any last name that has five characters and ends with "y", such as "Smithy" or "Jonesy".

```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE last_name LIKE 'b____y'
```

    This example demonstrates how to use the `LIKE` keyword to filter results based on a pattern. The query selects all customers whose last name has exactly five characters, starts with "b", and ends with "y". The `_` wildcard character represents a single character, so this will match any last name that has five characters, starts with "b", and ends with "y", such as "brushy" or "buzzy".

```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE address LIKE '%trail%' OR
	address LIKE '%avenue%';

```

    This example demonstrates how to use the `LIKE` keyword to filter results based on multiple patterns. The query selects all customers whose address contains either "trail" or "avenue". The `%` wildcard character represents zero or more characters, so this will match any address that contains "trail" or "avenue", regardless of its position in the string.

```sql
-- LIKE Keyword
SELECT *
FROM customers
WHERE phone NOT LIKE '%9';

```

    This example demonstrates how to use the `LIKE` keyword to filter results based on a pattern. The query selects all customers whose phone number does not end with "9". The `%` wildcard character represents zero or more characters, so this will match any phone number that does not end with "9", such as "123-456-7890" or "987-654-3210".
