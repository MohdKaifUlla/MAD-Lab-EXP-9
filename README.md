# 📱 Experiment 9 – Data Persistence using SharedPreferences and SQLite

## Develop an Android Application Using SharedPreferences and SQLite Database

---

## 👨‍💻 Author

**Name:** Mohammed Kaif Ulla  
**USN:** 25MCAR0226  
**Subject:** Mobile Application Development Lab

---

## 📖 Experiment Description

This experiment demonstrates data persistence in Android using **SharedPreferences** and **SQLite Database** (`SQLiteOpenHelper`) with Kotlin and XML.

The application provides an interactive interface for managing student records. It allows storing and retrieving student preferences (Student Name and USN) using SharedPreferences and performing CRUD (Create, Read, Delete) operations on structured student records stored in a local SQLite database.

Users can enter student details, save and load preferences, insert new student records, view all stored records, delete specific records using USN, and clear input/output fields.

### Scenario

The application simulates a **Student Information Data Management System**.

```text
          Student Data Manager App
                    ↓
            Enter Name and USN
                    ↓
          ┌─────────┴──────────┐
          ↓                    ↓
   SharedPreferences     SQLite Database
          ↓                    ↓
  ┌───────┴───────┐    ┌───────┼───────┐
  ↓               ↓    ↓       ↓       ↓
Save            Load  Insert  View   Delete
Prefs           Prefs Student Records Student
          └───────┬────────────┘
                  ↓
            Display Output
```

---

## 🧠 Concept / Technology Used

### SharedPreferences and SQLite Database

Android provides multiple data storage options depending on application needs. SharedPreferences is suitable for simple key-value pairs, while SQLite provides a lightweight relational database for managing structured data locally.

The application uses the following concepts:

- **SharedPreferences** – Stores key-value pairs persistently across application launches.
- **SQLite Database (`SQLiteOpenHelper`)** – Creates, manages, and executes SQL operations such as CREATE TABLE, INSERT, QUERY, and DELETE.
- **ContentValues & Cursor** – Used to construct database rows and retrieve query results.
- **Toast Messages** – Provides feedback to users after performing operations.
- **ScrollView & LinearLayout** – Creates a structured, scrollable user interface.
- **Kotlin** – Implements event handling, database operations, and preference management.
- **XML** – Defines the user interface components and layouts.
- **Android Studio** – Used for application development, building, and testing.

---

## 🚀 Features

- 🎓 Student Data Management Interface
- 👤 Input fields for Student Name and USN
- 💾 Save Student Details to SharedPreferences
- 📂 Load Saved Preferences from SharedPreferences
- ➕ Insert Student Records into SQLite Database
- 📜 View All Student Records
- 🗑️ Delete Specific Student Records by USN
- 🧹 Clear Input Fields and Output Area
- 💬 Toast Messages for User Operations
- 📱 Scrollable User Interface
- 🏷️ Footer displaying student details

---

## 📂 Project Structure

```text
app/
├── manifests/
│   └── AndroidManifest.xml
├── java/
│   └── com/
│       └── project/
│           └── exp9/
│               ├── MainActivity.kt
│               └── StudentDatabaseHelper.kt
├── res/
│   ├── layout/
│   │   └── activity_main.xml
│   └── values/
│       ├── colors.xml
│       ├── strings.xml
│       └── themes.xml
└── Gradle Scripts
```

---

## 🎨 User Interface

The application contains:

- Experiment header: Student Data Manager
- Input fields for Student Name and USN
- SharedPreferences section with Save Preferences and Load Preferences buttons
- SQLite Database section with Insert Student, View All Records, Delete by USN, and Clear Fields buttons
- Output display area showing operation results and database records
- Footer displaying author details (**Mohammed Kaif Ulla | USN: 25MCAR0226**)

---

## 🧪 Test Cases

### Test Case 1 – Save and Load SharedPreferences

**Objective:** Verify that student details can be saved to and loaded from SharedPreferences.

**Input:**
1. Enter Name: `Mohammed Kaif Ulla` and USN: `25MCAR0226`.
2. Tap **Save Preferences**.
3. Clear the fields or relaunch the application, then tap **Load Preferences**.

**Expected Result:** The student details should be saved in key-value format and loaded back into the input fields and output display.

**Actual Result:** The preferences can be saved and retrieved from SharedPreferences.

**Status:** ✅ Passed

---

### Test Case 2 – Insert and View Records in SQLite

**Objective:** Verify that student records can be inserted into the SQLite database and retrieved.

**Input:**
1. Enter student details.
2. Tap **Insert Student**.
3. Tap **View All Records**.

**Expected Result:** The student record should be inserted into the database, and all stored records should be displayed with their auto-generated IDs.

**Actual Result:** Records can be inserted and displayed in the output area.

**Status:** ✅ Passed

---

### Test Case 3 – Delete Record by USN and Clear Fields

**Objective:** Verify that a specific record can be deleted using USN and that input/output fields can be cleared.

**Input:**
1. Enter a USN and tap **Delete by USN**.
2. Tap **Clear Fields**.

**Expected Result:** The matching record should be removed from the SQLite database, and the input fields and output area should be cleared.

**Actual Result:** The record can be deleted, and fields can be cleared as expected.

**Status:** ✅ Passed

---

## 👨‍🎓 Student Details

**Name:** Mohammed Kaif Ulla  
**USN:** 25MCAR0226

**Experiment:** 9 – Data Persistence using SharedPreferences and SQLite
