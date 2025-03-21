# 📚 SQL Querying Basics

This document provides an overview of basic SQL queries used to retrieve and manipulate data from a database.

---

## 1. `SELECT select_list FROM table_name;`
- Retrieves data from the specified columns in a table.
- Basic query used to fetch desired information.
- `select_list` contains columns to display.

---

## 2. `SELECT first_name FROM customer;`
- Fetches the `first_name` column from the `customer` table.
- Displays only one specific column.
- Useful when you need data from a single column.

---

## 3. `SELECT first_name, last_name, email FROM customer;`
- Retrieves multiple columns (`first_name`, `last_name`, and `email`) from the `customer` table.
- Allows you to view related data together.
- Ideal for extracting selected fields.

---

## 4. `SELECT * FROM customer;`
- Retrieves all columns from the `customer` table.
- Displays every field and row in the table.
- Useful when all information is required.

---

## 5. `SELECT first_name || ' ' || last_name, email FROM customer;`
- Concatenates `first_name` and `last_name` with a space.
- Displays the full name and `email` for each record.
- Useful when combining multiple fields into one.

---

## 6. `SELECT first_name || ' ' || last_name full_name, email FROM customer;`
- Creates an alias `full_name` for the concatenated names.
- Simplifies data presentation with a meaningful name.
- Aliases improve query readability.

---

## 7. `SELECT column_name alias_name FROM table_name;`
- Assigns an alias (`alias_name`) to `column_name`.
- Aliases are useful for improving readability.
- Helps simplify long or complex column names.

---

## 8. `SELECT first_name || ' ' || last_name AS full_name FROM customer;`
- Uses `AS` to create an alias (`full_name`) for concatenated names.
- Makes result more understandable.
- `AS` is an optional keyword, but improves clarity.

---

## 9. `SELECT first_name, last_name FROM customer ORDER BY first_name ASC;`
- Retrieves customer names and sorts them by `first_name` in ascending order.
- `ORDER BY` controls the sorting order.
- `ASC` (ascending) is the default sort order.

---

## 10. `SELECT first_name, last_name FROM customer ORDER BY last_name DESC;`
- Retrieves names and sorts them by `last_name` in descending order.
- `DESC` sorts values from highest to lowest.
- Useful for reverse sorting.

---

## 11. `SELECT first_name, LENGTH(first_name) len FROM customer ORDER BY len DESC;`
- Retrieves `first_name` and its length using `LENGTH()`.
- Alias `len` is used to store the length value.
- Results are sorted by length in descending order.

---

## 12. `SELECT DISTINCT column1, column2 FROM table_name;`
- Returns unique combinations of `column1` and `column2`.
- Removes duplicate records from the result.
- Useful for identifying distinct pairs.

---

## 13. `SELECT DISTINCT column1, column2 FROM table_name;`
- Same as query 12, ensures distinct results.
- Prevents duplicate values in selected columns.
- Helps extract unique combinations.

---

## 14. `SELECT DISTINCT * FROM table_name;`
- Retrieves unique rows from the table.
- Removes duplicate entries from all columns.
- Ensures a clean and concise result set.

---

