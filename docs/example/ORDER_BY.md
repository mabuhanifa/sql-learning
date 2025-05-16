```sql
-- ORDER BY Keyword
SELECT *
FROM customers
ORDER BY first_name DESC;

```

    This example demonstrates how to use the `ORDER BY` keyword to sort the results of a query. The query selects all customers and orders them by their first name in descending order. The `DESC` keyword specifies that the results should be sorted in descending order, meaning that the names will be listed from Z to A.

```sql
-- ORDER BY Keyword
SELECT *
FROM order_items
WHERE order_id =2
ORDER BY quantity * unit_price DESC

```

    This example demonstrates how to use the `ORDER BY` keyword to sort the results of a query based on a calculated value. The query selects all order items for a specific order and orders them by the total price (quantity multiplied by unit price) in descending order. The `DESC` keyword specifies that the results should be sorted in descending order, meaning that the items with the highest total price will be listed first.

```sql
-- ORDER BY Keyword
SELECT * , quantity * unit_price AS total_price
FROM order_items
WHERE order_id =2
ORDER BY total_price DESC

```

    This example demonstrates how to use the `ORDER BY` keyword to sort the results of a query based on a calculated value. The query selects all order items for a specific order and orders them by the total price (quantity multiplied by unit price) in descending order. The `DESC` keyword specifies that the results should be sorted in descending order, meaning that the items with the highest total price will be listed first. The `AS` keyword is used to give the calculated column a name (`total_price`) for easier reference.
