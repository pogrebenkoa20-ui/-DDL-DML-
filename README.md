# Домашнее задание к занятию «Работа с данными (DDL/DML)» Погребенко Александр

### Задание 1
1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

<img width="755" height="432" alt="install" src="https://github.com/user-attachments/assets/60210cb2-a457-43ee-aea2-629f084475f8" />

.
<img width="747" height="231" alt="status" src="https://github.com/user-attachments/assets/1756c9f3-8222-4aa8-ad9f-cb1cec69797c" />


1.2. Создайте учётную запись sys_temp. 

<img width="687" height="82" alt="sys_temp" src="https://github.com/user-attachments/assets/bbe4acda-dce5-460b-9f9a-bf1c8ca84280" />



1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

<img width="561" height="215" alt="users" src="https://github.com/user-attachments/assets/4339fc47-953b-475f-8360-e18cc9e4941f" />

1.4. Дайте все права для пользователя sys_temp. 
<img width="733" height="111" alt="grant all" src="https://github.com/user-attachments/assets/4946f9f4-af6e-4488-b619-080a138df352" />


1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)
<img width="583" height="698" alt="privileges" src="https://github.com/user-attachments/assets/f979e3d8-0c2d-4011-8d28-254e9a7fa4df" />


1.6. Переподключитесь к базе данных от имени sys_temp.
<img width="637" height="331" alt="sys_temp user" src="https://github.com/user-attachments/assets/245bd99f-a8d3-4321-ae71-e8ae5bb5cec2" />

Для смены типа аутентификации с sha2 используйте запрос: 
```sql
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```
1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

<img width="745" height="288" alt="sakira" src="https://github.com/user-attachments/assets/eaf3632e-9af3-420a-87de-cd81a144e72f" />


1.7. Восстановите дамп в базу данных.
<img width="713" height="490" alt="source" src="https://github.com/user-attachments/assets/b442bd67-3e5f-4610-bc1f-667fbb4eae13" />

.
<img width="728" height="201" alt="source 2" src="https://github.com/user-attachments/assets/c1cd7ef2-284e-4603-9f8a-b0c150d20db4" />
.
<img width="497" height="203" alt="show" src="https://github.com/user-attachments/assets/b75f1c1e-36d4-4d58-9aa3-6677749c1ae5" />

1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)
<img width="503" height="458" alt="tables" src="https://github.com/user-attachments/assets/5e20d741-c257-488e-b73c-d4947acb5d4c" />



### Задание 2
Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)
```
Название таблицы | Название первичного ключа
customer         | customer_id
```
<img width="241" height="315" alt="table" src="https://github.com/user-attachments/assets/198bc5cf-528c-4ac9-a93f-c6560b06ba1c" />



