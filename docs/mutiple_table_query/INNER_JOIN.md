```sql
-- INNER JOIN
SELECT order_id, o.customer_id, first_name, last_name
FROM orders o
JOIN customers c
 ON o.customer_id = c.customer_id

```

This example demonstrates how to use the `INNER JOIN` clause to combine rows from two tables based on a related column between them. The query selects the order ID and customer ID from the `orders` table, as well as the first and last names from the `customers` table. The join condition specifies that the `customer_id` in the `orders` table must match the `customer_id` in the `customers` table. This will return only those orders that have a corresponding customer in the `customers` table.

```sql
-- INNER JOIN
SELECT order_id, oi.product_id, quantity, oi.unit_price
FROM order_items oi
JOIN products p ON oi.product_id = p.product_id

```

This example demonstrates how to use the `INNER JOIN` clause to combine rows from two tables based on a related column between them. The query selects the order ID, product ID, quantity, and unit price from the `order_items` table, as well as the product name from the `products` table. The join condition specifies that the `product_id` in the `order_items` table must match the `product_id` in the `products` table. This will return only those order items that have a corresponding product in the `products` table.
