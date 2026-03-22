# Enrollment Management System

A Java-based desktop application for managing student enrollments, courses, and records, integrated with a MySQL database.

## 📂 Project Structure

- **`src/`**: Contains the Java source code (.java files).
- **`lib/`**: Contains the required MySQL JDBC Driver (Connector).
- **`database/`**: Contains the `.sql` export file to recreate the database.
- **`EnrollmentSystem.jar`**: The executable application file.

---

## 🛠️ How to Set Up the MySQL Database

Before running the app, you must set up the database in **MySQL Workbench**:

1. **Open MySQL Workbench** and connect to your local instance.
2. **Create a New Schema**: Click the "Create a new schema" icon and name it `enrollment_system`.
3. **Import Data**:
   - Go to **Server** > **Data Import**.
   - Select **Import from Self-Contained File**.
   - Browse and select the `enrollment_system.sql` file from this repository.
   - Select `enrollment_system` as the **Default Target Schema**.
   - Click **Start Import**.
4. **Verify**: Ensure the tables (`student`, `course`, `enrolled_subject`) appear under the schema.

---

## 🚀 How to Run the Application

### Option 1: Double-Click (Easiest)
1. Ensure you have **Java (JDK 17 or later)** installed.
2. Ensure the `lib` folder is in the same directory as the `EnrollmentSystem.jar`.
3. Double-click `EnrollmentSystem.jar`.

### Option 2: Command Line (If double-click doesn't work)
Open Terminal or PowerShell in the project folder and run:
```bash
java -jar EnrollmentSystem.jar
