1) Выберите из таблицы orders все заказы

SELECT * FROM orders;

![image](https://github.com/user-attachments/assets/b7abd3bc-6786-405a-ac5e-429b02cf5a38)

2) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in

SELECT * FROM orders WHERE status IN ('in_progress', 'cancelled', 'delivery');

![image](https://github.com/user-attachments/assets/9a13c6b2-2445-47da-ae68-2946272823b7)

3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".

SELECT * FROM orders WHERE status IN ('new', 'cancelled');

![image](https://github.com/user-attachments/assets/4e573f01-acf9-4aba-b3dc-54ac94fba874)

4) Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа.

SELECT id, sum FROM orders WHERE products_count >3;

![image](https://github.com/user-attachments/assets/dbf274a3-2fbd-42d8-acf1-a25e6717015b)
