use ecommerce;

/*EX1*/
SELECT order_id, order_date, first_name, last_name, email
FROM orders
INNER JOIN Customers
ON Customers.customer_id = orders.order_id;

/*EX 2*/
SELECT product_name, quantity
FROM Products
INNER JOIN order_items
ON Products.product_id = Order_Items.product_id
INNER JOIN orders
ON Order_items.order_id = Orders.order_id
WHERE customer_id = 1;

/*EX 3*/
SELECT first_name, last_name, SUM(quantity)*SUM(price)
FROM customers
INNER JOIN orders
ON customer_id.customers = customer_id.orders
INNER JOIN order_items
ON  order_id.orders = order_id.order_items
INNER JOIN products
ON  product_id.order_items = product_id.products;  
