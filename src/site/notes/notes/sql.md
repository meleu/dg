---
{"dg-publish":true,"permalink":"/notes/sql/"}
---

# SQL


## Source of Information

Some notes here were taken while studying the first lessons of "SQL Fundamentals" from <datacamp.com>

Others were taken by demand.


## SELECT with Regular Expressions

**NOTE**: I only tested this on MySQL.

```sql
SELECT 
  column_list
FROM
  table_name
WHERE
  string_column REGEXP pattern;
```

example:
```sql
SELECT 
  productname
FROM
  products
WHERE
  productname REGEXP '^(A|B|C)'
ORDER BY productname;
```



## SELECT DISTINCT

Works like `uniq` in shell scripts.

## SELECT COUNT()

### COUNT(*)

Counts the number of rows.

### COUNT(column_name)

Counts the number of *non-missing* values in `column_name`.

### COUNT(DISTINCT column_name)

Counts the number of distinct values in `column_name`.

## WHERE

### WHERE a BETWEEN x AND y

Checks if the value of `a` is between the values `x` and `y` (inclusive).

### WHERE a IN (value1, value2, value3)

Checks if `a` is equal one of the values in the list.

### SELECT a LIKE pattern / SELECT a NOT LIKE pattern

Allows using patterns for searching.

`%` is a wildcard fro "anything", and `_` is a wildcard forr any character).


## Aggregate functions

### SELECT AVG()

### SELECT SUM()

### SELECT MAX()

### SELECT MIN()


## RA Practice

![basic RA DB scheme](https://user-images.githubusercontent.com/8508804/92043707-f1ea8080-ed52-11ea-9f3e-e5fbb3caf616.png)


### How many users have less than 1000 points?

```sql
SELECT COUNT(*)
FROM UserAccounts
WHERE RAPoints < 1000;
```

### How many users don't log in for more than 2 years?

```sql
SELECT COUNT(*)
FROM UserAccounts
WHERE LastLogin < ??????(timestamp)
```

### How many users have created at least one achievement?

```sql
SELECT COUNT(DISTINCT Author)
FROM Achievements;
```

### How many users didn't create any achievement?

???


### How many users have less than 1000 points AND didn't login for 2 years AND didn't create any achievement?

```sql
SELECT COUNT(*)
FROM UserAccounts
WHERE
  RAPoints < 1000
  AND LastLogin < ??????(timestamp)
  AND ?????;
```

### Which users have less than 1000 points AND didn't login for 2 years AND didn't create any achievement?

```sql
SELECT User
FROM UserAccounts
WHERE
  RAPoints < 1000
  AND LastLogin < ??????(timestamp)
  AND ?????;
```

### How many points the user USERNAME had in the date X?

???

NOTE: rescores won't allow it to be accurate.


---


https://twitter.com/Aakriti_Sarma/status/1586183550260240385?s=20&t=FPX6eR-Itt6wPoX7MLGMVg