# Copy table in MYSQL

## With data

```sql
CREATE TABLE `tab2` SELECT * FROM `tab1`;
```

## Without data

```sql
CREATE TABLE `tab2` LIKE `tab1`;
```

OR

```sql
CREATE TABLE `guests` SELECT * FROM `users` WHERE 0;
ALTER TABLE `guests` ADD PRIMARY KEY (`id`);
ALTER TABLE `guests` CHANGE `id` `id` INT(10) UNSIGNED NOT NULL AUTO_INCREMENT;
```