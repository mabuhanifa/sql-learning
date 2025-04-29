```sql
-- AS Keyword
SELECT name, unit_price,unit_price*1.1 AS new_price from products;
```

This query selects the `name` and `unit_price` columns from the `products` table, and it calculates a new price by multiplying the `unit_price` by 1.1. The result of this calculation is given an alias of `new_price` using the `AS` keyword. This means that in the result set, the calculated column will be labeled as `new_price`.
