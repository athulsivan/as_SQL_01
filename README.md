
# 🐘 SQL Learning and Practice Repository

Welcome to the **SQL Practice** repository!  
This space is dedicated to learning, experimenting with, and mastering SQL (Structured Query Language) — the language of relational databases. Whether starting from scratch or brushing up on key concepts, this guide and project structure are here to help.

---

## 📚 Table of Contents

1. [📌 About This Repository](#-about-this-repository)  
2. [💾 Setting Up a SQL Environment](#-setting-up-a-sql-environment)  
3. [🔤 SQL Basics: Syntax & Concepts](#-sql-basics-syntax--concepts)  
4. [🧪 Practice Exercises](#-practice-exercises)  
5. [🗂 Folder Structure](#-folder-structure)  
6. [📘 Recommended Learning Resources](#-recommended-learning-resources)  
7. [💡 Tips for Learning SQL](#-tips-for-learning-sql)  
8. [🧾 License](#-license)

---

## 📌 About This Repository

This repository is a structured, hands-on guide to SQL. It includes:

- Installation guides for SQLite, MySQL, and PostgreSQL.
- Example scripts and practice queries.
- Beginner to intermediate exercises with solutions.
- Support for importing sample datasets (CSV or SQL).

Use this repo to:

- Learn core SQL syntax and commands.
- Practice creating and querying tables.
- Understand real-world database design.
- Build muscle memory through repetition and experimentation.

---

## 💾 Setting Up a SQL Environment

Choose one of the following SQL engines:

### ✅ SQLite (Recommended for Beginners)
- Lightweight, no setup needed beyond installation.
- Stores database as a single `.db` file.

**Installation:**

```bash
# Linux
sudo apt update
sudo apt install sqlite3

# macOS (with Homebrew)
brew install sqlite

# Windows / All platforms:
Download from https://www.sqlite.org/download.html
```

**Check Installation:**
```bash
sqlite3 --version
```

---

## 🔤 SQL Basics: Syntax & Concepts

### 🗃️ Core Concepts
| Term       | Meaning                                       |
|------------|-----------------------------------------------|
| Database   | A structured collection of data               |
| Table      | A grid with rows and columns storing records  |
| Row        | A single record (like one student)            |
| Column     | A data field (like "name" or "age")           |

### 🧾 Common SQL Statements
```sql
CREATE TABLE students (
    id INTEGER PRIMARY KEY,
    name TEXT,
    age INTEGER
);

INSERT INTO students (name, age) VALUES ('Alice', 21);
SELECT * FROM students;
UPDATE students SET age = 22 WHERE name = 'Alice';
DELETE FROM students WHERE name = 'Alice';
```

---

## 🧪 Practice Exercises

Try to solve these on your own. Solutions are available in the `sql/solutions` folder.

### 📘 Exercise 1: Books Table
- Create a table: `books (id, title, author, year)`
- Insert 3+ sample books
- Select books published after 2010
- Update the author of one book
- Delete a book by title

### 📗 Exercise 2: Employees
- Table: `employees (id, name, department, salary)`
- Insert multiple records
- Query employees by department
- Find top-paid employee
- Increase salary by 10% for all

Add your own exercises in the `sql/exercises/` folder!

---

## 🗂 Folder Structure

```
.
├── README.md               # This guide
├── LICENSE                 # Open-source license (MIT)
├── requirements.txt        # Optional Python dependencies
│
├── sql/
│   ├── basics/             # Basic SQL queries
│   ├── exercises/          # Practice problems
│   └── solutions/          # Suggested answers
│
├── sqlite/                 # SQLite setup and starter DB
├── mysql/                  # MySQL scripts
├── postgres/               # PostgreSQL scripts
│
├── data/                   # CSV or sample data files
└── notebooks/              # Jupyter notebooks (optional)
```

---

## 📘 Recommended Learning Resources

- 🐘 [SQLZoo](https://sqlzoo.net/)
- 🧠 [Mode SQL Tutorial](https://mode.com/sql-tutorial/)
- 💡 [W3Schools SQL Guide](https://www.w3schools.com/sql/)
- 🧪 [HackerRank SQL Challenges](https://www.hackerrank.com/domains/tutorials/10-days-of-statistics)
- 🧮 [LeetCode SQL Problems](https://leetcode.com/problemset/database/)

---

## 💡 Tips for Learning SQL

- Practice small queries every day.
- Don't memorize; understand the logic behind each command.
- Always test edge cases (e.g., NULLs, duplicates).
- Break problems into steps: SELECT → WHERE → GROUP → JOIN
- Use real datasets to make it interesting.

---

## 🧾 License

This project is licensed under the [MIT License](LICENSE).

---

Happy querying! 🌟
