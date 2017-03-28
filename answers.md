## Example:
1.
 - `SQL:`
    SELECT count(\*) from items

 - `ANSWER:`
   100

---

1.
 - `SQL:`
 SELECT "count"(id) FROM users;
 - `ANSWER:`
 50

2.What are the titles of the 5 most expensive items?
 - `SQL:` SELECT *  FROM items ORDER BY price DESC  LIMIT 5;

 - `ANSWER:` Multi-layered modular service-desk, Re-engineered fault-tolerant adapter, Upgradable 24/7 access, Quality-focused heuristic info-mediaries, Enterprise-wide secondary firmware

 3.What's the cheapest item in the Books category?
 - 'SQL:' select * FROM items WHERE category = 'Books' order by price LIMIT 1;

 - 'ANSWER:'Ergonomic Granite Chair

 4. Who lives at 6439 Zetta Hills, Willmouth, WY?
 - 'SQL: select users.first_name, users.last_name FROM users, addresses WHERE users.id = addresses.user_id and street = '6439 Zetta Hills' and city = 'Willmouth' and state = 'WY';

 - 'ANSWER:'| Corrine      | Little   

 5. Correct Virginie Mitchell's address to "New York, NY, 10108".
 - 'SQL:' UPDATE addresses SET city = 'New York', state = 'NY', zip = 10108 WHERE user_id = 39;

 - 'ANSWER:' done.

 6. How much would it cost to buy one of each item in the Tools category?
 - 'SQL:'  SELECT "sum"(price) FROM items WHERE category = 'Tools';

 - 'ANSWER:' 7383

 7. How many total items did we sell?
 - 'SQL:' SELECT "sum"(quantity) FROM orders;

 - 'ANSWER:' 2125

 8. How much was spent on Books?
 - 'SQL:'  SELECT "sum"(quantity), "sum"(price) FROM orders, items WHERE orders.item_id = items.id and items.category = 'Books';

 - 'ANSWER:' $68982

 9. Simulate buying an item by inserting a User for yourself and an Order for yourself.
 - 'SQL:' insert INTO users VALUES (51, 'Patrick', 'Miller', 'pjmiller823@gmail.com');
  INSERT INTO orders VALUES (377, 51, 66, 4, '2015-02-10  00:40:31.307668');

 - 'ANSWER:'
