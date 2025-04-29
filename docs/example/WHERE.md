id --- first_name --- last_name ---- birth_date ---- phone address ---- city --- state --- points
'1', 'Babara', 'MacCaffrey', '1986-03-28', '781-932-9754', '0 Sage Terrace', 'Waltham', 'VA', '2273'
'2', 'Ines', 'Brushfield', '1986-04-13', '804-427-9456', '14187 Commercial Trail', 'Hampton', 'VA', '947'
'3', 'Freddi', 'Boagey', '1985-02-07', '719-724-7869', '251 Springs Junction', 'Colorado Springs', 'CO', '2967'
'4', 'Ambur', 'Roseburgh', '1974-04-14', '407-231-8017', '30 Arapahoe Terrace', 'Orlando', 'FL', '457'
'5', 'Clemmie', 'Betchley', '1973-11-07', NULL, '5 Spohn Circle', 'Arlington', 'TX', '3675'
'6', 'Elka', 'Twiddell', '1991-09-04', '312-480-8498', '7 Manley Drive', 'Chicago', 'IL', '3073'
'7', 'Ilene', 'Dowson', '1964-08-30', '615-641-4759', '50 Lillian Crossing', 'Nashville', 'TN', '1672'
'8', 'Thacher', 'Naseby', '1993-07-17', '941-527-3977', '538 Mosinee Center', 'Sarasota', 'FL', '205'
'9', 'Romola', 'Rumgay', '1992-05-23', '559-181-3744', '3520 Ohio Trail', 'Visalia', 'CA', '1486'
'10', 'Levy', 'Mynett', '1969-10-13', '404-246-3370', '68 Lawn Avenue', 'Atlanta', 'GA', '796'

```sql
-- SELECT Keyword
SELECT * FROM customers WHERE points>3000;
```

This query selects all columns from the `customers` table where the `points` column is greater than 3000. The `WHERE` clause filters the rows based on the specified condition, so only customers with more than 3000 points will be included in the result set.

```sql
-- SELECT Keyword
SELECT * FROM orders WHERE order_date>= "2019-01-01";
```

This query selects all columns from the `orders` table where the `order_date` is greater than or equal to January 1, 2019. The `WHERE` clause filters the rows based on the specified condition, so only orders placed on or after that date will be included in the result set.

```sql
-- SELECT Keyword
SELECT *
FROM customers
WHERE NOT (birth_date > "1990-01-01" OR
	points > 1000)
```

This query selects all columns from the `customers` table where the `birth_date` is not greater than January 1, 1990, and the `points` are not greater than 1000. The `WHERE` clause filters the rows based on the specified condition, so only customers who do not meet either of these criteria will be included in the result set.

```sql
-- SELECT Keyword
SELECT *
FROM order_items
WHERE order_id = 6 AND unit_price * quantity > 30
```

This query selects all columns from the `order_items` table where the `order_id` is equal to 6 and the product of `unit_price` and `quantity` is greater than 30. The `WHERE` clause filters the rows based on the specified conditions, so only order items that meet both criteria will be included in the result set.
