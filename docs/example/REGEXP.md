```sql
-- REGEXP Keyword
SELECT *
FROM customers
WHERE last_name REGEXP 'field$|mac|rose'
```

This example demonstrates how to use the `REGEXP` keyword to filter results based on a regular expression pattern. The query selects all customers whose last name ends with "field", contains "mac", or contains "rose". The `$` symbol indicates the end of the string, and the `|` symbol acts as an OR operator, allowing for multiple conditions.

```sql
-- REGEXP Keyword
SELECT *
FROM customers
WHERE last_name REGEXP '[gim]e'

```

This example demonstrates how to use the `REGEXP` keyword to filter results based on a regular expression pattern. The query selects all customers whose last name contains either "g", "i", or "m" followed by "e". The square brackets `[]` indicate a character class, allowing for multiple characters to match.

```sql
-- REGEXP Keyword
SELECT *
FROM customers
WHERE last_name REGEXP '[a-h]e'
```

This example demonstrates how to use the `REGEXP` keyword to filter results based on a regular expression pattern. The query selects all customers whose last name contains either "a", "b", "c", "d", "e", "f", "g", or "h" followed by "e". The square brackets `[]` indicate a character class, allowing for multiple characters to match.

```sql
-- REGEXP Keyword
SELECT *
FROM customers
WHERE first_name REGEXP 'elka|ambur'
OR last_name REGEXP 'ey$on$'
OR last_name REGEXP '^my|se'
OR last_name REGEXP 'b[ru]'
```

This example demonstrates how to use the `REGEXP` keyword to filter results based on multiple regular expression patterns. The query selects all customers whose first name contains "elka" or "ambur", last name ends with "ey" or "on", last name starts with "my" or contains "se", or last name contains "b" followed by either "r" or "u". The `|` symbol acts as an OR operator, allowing for multiple conditions.
