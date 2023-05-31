# MySQL Interview Questions And Answers

Most targeted up-to-date MySQL interview questions and answers list

# Table of Contents

1. [What is a query in MySQL?](#1-what-is-a-query-in-mysql)
2. [How do you create a basic select query in MySQL?](#2-how-do-you-create-a-basic-select-query-in-mysql)
3. [What is a parameterized query in MySQL?](#3-what-is-a-parameterized-query-in-mysql)
4. [How can you calculate a field's value in a MySQL query?](#4-how-can-you-calculate-a-fields-value-in-a-mysql-query)
5. [What is a join in MySQL?](#5-what-is-a-join-in-mysql)
6. [What is a subquery in MySQL?](#6-what-is-a-subquery-in-mysql)
7. [How do you sort query results in ascending or descending order in MySQL?](#7-how-do-you-sort-query-results-in-ascending-or-descending-order-in-mysql)
8. [What is a wildcard character in MySQL queries?](#8-what-is-a-wildcard-character-in-mysql-queries)
9. [How do you use a wildcard in a MySQL query?](#9-how-do-you-use-a-wildcard-in-a-mysql-query)
10. [What is a limit query in MySQL?](#10-what-is-a-limit-query-in-mysql)
11. [How do you perform grouping and aggregate functions in MySQL?](#11-how-do-you-perform-grouping-and-aggregate-functions-in-mysql)
12. [What is a self-join in MySQL?](#12-what-is-a-self-join-in-mysql)
- [Whats more?](#whats-more)
- [Contributing](#contributing)
- [License](#license)

## 1. What is a query in MySQL?

In MySQL, a query is a request for data retrieval or manipulation from one or more tables in a database. It allows you to filter, sort, calculate, and summarize data based on specific criteria.

## 2. How do you create a basic select query in MySQL?

To create a select query in MySQL, you can use the SELECT statement. Here's an example:

```sql
SELECT column1, column2 FROM tableName;
```

## 3. What is a parameterized query in MySQL?

A parameterized query in MySQL allows you to pass dynamic values as parameters into your query. It helps prevent SQL injection and provides flexibility. Here's an example:

```sql
SELECT column1, column2 FROM tableName WHERE column1 = :parameter;
```

## 4. How can you calculate a field's value in a MySQL query?

You can use calculated fields in MySQL queries to perform calculations on existing data or combine multiple fields. Here's an example that calculates the total price based on unit price and quantity:

```sql
SELECT productName, unitPrice, quantity, (unitPrice * quantity) AS totalPrice FROM tableName;
```

## 5. What is a join in MySQL?

In MySQL, a join combines records from two or more tables based on a related column between them. It allows you to retrieve data from multiple tables simultaneously. Here's an example of an inner join:

```sql
SELECT column1, column2 FROM table1 INNER JOIN table2 ON table1.column = table2.column;
```

## 6. What is a subquery in MySQL?

A subquery in MySQL is a query nested inside another query. It is used to retrieve data based on the results of an inner query. Here's an example:

```sql
SELECT column1, column2 FROM tableName WHERE column1 IN (SELECT column1 FROM subTable);
```

## 7. How do you sort query results in ascending or descending order in MySQL?

To sort query results in MySQL, you can use the ORDER BY clause followed by the column name and the keywords ASC (ascending) or DESC (descending). Here's an example:

```sql
SELECT columnName FROM tableName ORDER BY columnName ASC;
```

## 8. What is a wildcard character in MySQL queries?

In MySQL, a wildcard character is a special symbol used in query patterns to match one or more characters. The percentage sign (%) represents multiple characters, and the underscore (_) represents a single character.

## 9. How do you use a wildcard in a MySQL query?

You can use the LIKE operator along with wildcard characters to filter data based on specific patterns in MySQL. Here's an example:

```sql
SELECT columnName FROM tableName WHERE columnName LIKE 'A%';
```

## 10. What is a limit query in MySQL?

A limit query in MySQL allows you to restrict the number of records returned by a query. It is used to retrieve a specific number of rows. Here's an example:

```sql
SELECT columnName FROM tableName LIMIT 10;
```

## 11. How do you perform grouping and aggregate functions in MySQL?

In MySQL, you can use the GROUP BY clause along with aggregate functions such as SUM, COUNT, AVG, etc., to perform calculations on grouped data. Here's an example:

```sql
SELECT column1, SUM(column2) FROM tableName GROUP BY column1;
```

## 12. What is a self-join in MySQL?

A self-join in MySQL occurs when a table is joined with itself based on a related column. It is useful when you need to combine records within the same table. Here's an example:

```sql
SELECT t1.column1, t2.column2 FROM tableName t1 INNER JOIN tableName t2 ON t1.column = t2.column;
```

## What's more?
<a href="https://interviewplus.ai/database-administration/mysql/questions">A comprehensive list of questions and answers</a>

## Contributing
We welcome contributions from our users to help make this resource as comprehensive and useful as possible. If you have been recently interviewed and encountered a question that is not currently covered on our website, feel free to suggest it as a new question. Your contributions will be added to our platform, and we will make sure to credit you for your contributions. We appreciate your help in making our platform a valuable tool for all job seekers.

## License
MIT License
