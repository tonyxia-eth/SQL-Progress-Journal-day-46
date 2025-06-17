# Day 46 – Hacking with Python & SQL 🔐🐍

## Project: `dont-panic.db` Penetration Test

As part of CS50’s Introduction to Databases with SQL (Week 6), I completed a hands-on assignment simulating a penetration test using Python and SQL.

### 🎯 Objective
To demonstrate how to:
- Connect to a SQLite database using Python
- Execute SQL statements via Python
- Perform secure updates using **prepared statements**

### 🧪 Task Breakdown
1. Connected Python to `dont-panic.db` using the `cs50` library.
2. Wrote a script (`hack.py`) to update the `admin` user's password.
3. Took user input in the script and used a **prepared SQL statement** to change the admin password.
4. Validated the change by inspecting the database manually using `sqlite3`.

### 💻 Commands Used

```bash
# Ran the script
python hack.py

# Manually confirmed the update
sqlite3 dont-panic.db
SELECT * FROM users;


🧠 Skills Demonstrated
SQL injection safety with prepared statements

Automating SQL tasks with Python

Securely altering data in SQLite

Cross-technology scripting

🔐 Before & After
User	Field	Value
admin	password	poopoo (updated by script)

📁 Files
hack.py – Python script to update user passwords

dont-panic.db – Target SQLite database
