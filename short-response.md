# Short Response: SQL Basics

Answer each question below. Write in complete sentences (3–5 per answer).

---

## Question 1

What is a database? Why do we use one instead of storing data in a JavaScript array on your server?

**Your answer:**

A database is an organized collection of data that is easy to search through. An example of a database is a library, which contains data on all its books currently available in its inventory, allowing users to find the book they are looking for. Databases are better at storing data because they are persistent, preventing data corruption even when servers are shut down due to updates, crashes, or restarts.
---

## Question 2

What is a primary key? Why does every table need one?

**Your answer:**

---

## Question 3

In one sentence, describe what this query does in plain English:

```sql
SELECT * FROM books WHERE genre = 'fiction' ORDER BY year DESC LIMIT 5;
```

Aim for something like: *"It returns the 5 most recently published fiction books."*

**Your answer:**

---

## Question 4

Why is it dangerous to run `DELETE FROM books` without a `WHERE` clause? What does it actually do?

**Your answer:**

---

## Question 5

What is the difference between `ORDER BY` and `LIMIT`? Could you use one without the other? Give an example to support your answer.

**Your answer:**
