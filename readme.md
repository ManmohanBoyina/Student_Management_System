# Student Management System (Console-Based)

A simple and intuitive **Console-Based Student Management System** developed in **C#** using **.NET SDK 7.0**. This application allows you to manage student records, including creating, updating, deleting students, assigning courses, entering marks, calculating GPA, and viewing available courses and departments. The system connects to a **Microsoft SQL Server (SQL Express 2022)** database.

---

## Features

✅ **Create Student**  
Add a new student by entering their ID, first name, last name, date of birth, and department ID.

✅ **Show Students**  
View a list of all students along with their basic information (name, date of birth, department ID).

✅ **Update Student**  
Modify an existing student's details by entering their ID and updating their information.

✅ **Delete Student**  
Remove a student record by providing their ID.

✅ **Add Course to Student**  
Assign one or more courses to a student by selecting their student ID and a course ID.

✅ **Insert Marks & Calculate GPA**  
Enter student marks for each course, and the system will automatically calculate their GPA.

✅ **Search Student**  
Find a student by their ID and display their full details, including enrolled courses and grades.

✅ **View Courses & Departments**  
See all available courses and departments. You can also add new ones.

---

## Technologies Used

- **C#**
- **.NET SDK 7.0.403**
- **Microsoft SQL Server (SQL Express 2022)**
- **Microsoft.Data.SqlClient (5.1.2)**

---

## Prerequisites

- [.NET SDK 7.0.403](https://dotnet.microsoft.com/en-us/download/dotnet/7.0)
- [Microsoft SQL Server Express 2022](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- Visual Studio Code (recommended) or Visual Studio
- C# Dev Kit Extension for VS Code (optional)

---

## Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <project-folder>
```

### 2. Database Setup
- **Option 1**: Create a new database manually in SQL Server.
- **Option 2**: Import the provided database backup file (if available).

### 3. Configure Database Connection
Edit the connection string in `Program.cs`:
```csharp
static string connectionString = "Data Source=localhost,51609;Initial Catalog=StudentManagementSystem;Integrated Security=True;Encrypt=False";
```
> ⚠️ Update `Data Source` and `port` according to your SQL Server instance.

If using SQL Server Configuration Manager:
- Enable TCP/IP protocol:  
  `SQL Server Network Configuration > Protocols for SQLEXPRESS > TCP/IP > Properties > IP Address`  
- Ensure TCP/IP is enabled and specify the correct port (e.g., 51609).

---

## Running the Project

### Using Visual Studio Code
1. Open the folder in VS Code.
2. Install the **C# Dev Kit** if you haven't already.
3. Restore dependencies:
   ```bash
   dotnet restore
   ```
4. Run the application:
   ```bash
   dotnet run
   ```

### Using Visual Studio
1. Open the solution in Visual Studio.
2. Restore NuGet packages.
3. Run the project using the debugger or `Ctrl + F5`.

---

## Error Handling & Troubleshooting

### Package Restore Issues
If packages are not restored automatically:
```bash
dotnet restore
```
Or manually add the `Microsoft.Data.SqlClient` package:
```bash
dotnet add package Microsoft.Data.SqlClient
```
[NuGet Package Link](https://www.nuget.org/packages/Microsoft.Data.SqlClient)

### SQL Server Connection Errors
- Check if your SQL Server instance is running.
- Verify that TCP/IP is enabled and the correct port is configured.
- Ensure your connection string in `Program.cs` is correct.

Example connection string:
```csharp
// Integrated Security (Windows Authentication)
static string connectionString = "Data Source=localhost,51609;Initial Catalog=StudentManagementSystem;Integrated Security=True;Encrypt=False";
```

---

## Future Improvements

- Implement a Graphical User Interface (GUI)
- Add Student Enrollment Management features
- Generate Grade Reports
- Provide Data Analytics & Insights
- Export data to PDF/CSV formats

---

## License

This project is licensed under the MIT License. Feel free to use, modify, and share.

---

## Author

Developed by [Your Name]  
For any queries or suggestions, feel free to reach out!

```

Let me know if you want to:
- Include setup screenshots
- Add database schema details
- Customize author/contact info
