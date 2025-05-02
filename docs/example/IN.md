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
-- In Keyword
SELECT *
FROM customers
-- WHERE state ="VA" OR state = "GA" OR state = "FL";
WHERE state IN ("VA","FL","GA");
```

This query selects all columns from the `customers` table where the `state` is either "VA", "FL", or "GA". The `IN` operator allows you to specify multiple values in a `WHERE` clause, making it easier to filter rows based on a list of possible values.

```sql
-- In Keyword
SELECT *
FROM products
WHERE quantity_in_stock IN (49,38,72);
```

This query selects all columns from the `products` table where the `quantity_in_stock` is either 49, 38, or 72. The `IN` operator allows you to specify multiple values in a `WHERE` clause, making it easier to filter rows based on a list of possible values.
