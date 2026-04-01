# Short Response: SQL Basics

Answer each question below. Write in complete sentences (3–5 per answer).

---

## Question 1

What is a database? Why do we use one instead of storing data in a JavaScript array on your server?

**Your answer:**

A **database** is an organized **collection of data** that is easy to search through. An example of a database is a **library**, which contains data on all its books currently **available** in its inventory, allowing users to find the book they are looking for. Databases are better at **storing data** because they are persistent, preventing data corruption or error when servers shut down due to updates, crashes, or restarts.
---

## Question 2

What is a primary key? Why does every table need one?

**Your answer:**

A **primary key** is a special column that **identifies** each record in the table, usually named after the data table. Primary key values are **sequential values** and are used to prevent **error** and **confusion**.
---

## Question 3

In one sentence, describe what this query does in plain English:

```sql
SELECT * FROM books WHERE genre = 'fiction' ORDER BY year DESC LIMIT 5;
```

Aim for something like: *"It returns the 5 most recently published fiction books."*

**Your answer:**

`SELECT * FROM books`: **Look into** the books' table data.
`WHERE genre = 'fiction'`: **gather** all fictional books.
`ORDER BY year DESC`: Then **sort** the books by the year it was **published**.
`LIMIT 5`: And return the **five most** recent books.
---

## Question 4

Why is it dangerous to run `DELETE FROM books` without a `WHERE` clause? What does it actually do?

**Your answer:**

`DELETE` removes rows from a table. `WHERE` tells the computer the **specific** data that needs to be removed from the table. Using `DELETE` without a `WHERE` clause, the computer to assume all rows, which leads to the computer removing **all** data from the table.
---

## Question 5

What is the difference between `ORDER BY` and `LIMIT`? Could you use one without the other? Give an example to support your answer.

**Your answer:**

`ORDER BY` **sort** your requested data by a variable in the database.

Example:
```sql
SELECT * FROM students ORDER BY grade DESC;
```
`LIMIT` **reduces** the amount of data returned to a request.

Example:
```sql
SELECT * FROM students LIMIT 3;
```
**Both** can be used on their **own**, but they can be used **together** for a more precise request.

Example:
```sql
SELECT * FROM students ORDER BY grade DESC LIMIT 3;
```
