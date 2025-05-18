# 🎓 Student Performance Tracker (SQLite + VS Code)
A beginner-friendly SQL project that demonstrates how to create a relational database to manage student performance. This project includes creating tables for students, subjects, and marks, inserting sample data, and running SQL queries to retrieve and analyze results.

## 📁 Project Structure: 💡 Features

- Create and manage relational tables (`Students`, `Subjects`, `Marks`)
- Insert sample student and marks data
- Run SQL JOIN queries to retrieve performance reports

## ⚙️ Setup Instructions: ✅ Prerequisites

- VS Code Installed
- SQLite extension installed in VS Code (e.g., `SQLite Viewer`)
- SQLite database file (`student_performance.db`)

### 🚀 Steps

1. Open the project folder in VS Code.
2. Install the SQLite extension (Search: `SQLite Viewer`).
3. Right-click on `student_performance.db` → **Open Database**.
4. Open `setup.sql` and paste the code from the project.
5. Select all SQL code → Right-click → **Execute Query**.

---

## 📊 Sample Output

Example query:

```sql
SELECT s.name, s.class, sub.subject_name, m.marks_obtained
FROM Students s
JOIN Marks m ON s.student_id = m.student_id
JOIN Subjects sub ON m.subject_id = sub.subject_id;
🔽 Output:
| Name    | Class | Subject | Marks |
| ------- | ----- | ------- | ----- |
| Alice   | 10A   | Math    | 88    |
| Alice   | 10A   | Science | 92    |
| Bob     | 10B   | Math    | 76    |
| Bob     | 10B   | English | 85    |
| Charlie | 10A   | Science | 90    |
| Charlie | 10A   | English | 87    |

