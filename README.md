🚀 Features

🔹 Student Management
Add, view, and list students
Registration dates handled with Java Date/Time API

🔹 Course Management
Create and list courses
Course creation implemented using the Builder Pattern

🔹 Enrollment Management
Enroll students in courses
Prevents duplicate enrollments with custom exceptions

🔹 Grade Management
Assign and display grades
Grades stored as Enum with grade points

🔹 Backup Utility
Creates timestamped backup folders
Uses Java NIO.2 (Files, Path) and recursion for directory size checks

🔹 Command-Line UI
Simple menu-driven interface for easy navigation


🧰 Technologies & Concepts Used

| Concept       | Implementation                                       |
| ------------- | ---------------------------------------------------- |
| Encapsulation | `Person.java`, `Student.java`                        |
| Inheritance   | `Student` & `Instructor` extend `Person`             |
| Abstraction   | `Person.java` (abstract class with `getDetails()`)   |
| Polymorphism  | Enrollment & course display using overridden methods |


 Design Patterns


Singleton: DataStore.java


Builder Pattern: Course.java (CourseBuilder)


✔ Core Java Features


Custom Exceptions (DuplicateEnrollmentException.java)


Streams API & Lambda Expressions


NIO.2 File I/O (BackupService, ImportExportService)


Date-Time API (LocalDateTime)


Recursion (Files.walk())


Organized packages: edu.ccrm.cli, edu.ccrm.domain, edu.ccrm.service



🛠 Installation & Setup

 Requirements


Java 17 or higher


Any IDE: VS Code, Eclipse, IntelliJ, etc.


 Clone the Repository
git clone https://github.com/JK-BB/CCRM_final.git

 Running the Project (VS Code Example)


Install Extension Pack for Java in VS Code


Open the project folder


Navigate to: src/edu/ccrm/cli/Main.java


Click Run ▶ to start the application



▶ How to Use the Application

Main Menu Options:
1 → Student Management
2 → Course Management
3 → Enrollment Management
4 → Grade Management
5 → Backup Utility
9 → Exit

Example Flow:


Press 1 → Student Menu


Press 1 → Add student → Enter details


Press 2 → List students


Press 9 → Return to main menu



🧪 Enabling Assertions (Optional)

assert student.getId() > 0 : "Student ID must be positive";

To enable assertions in VS Code, edit .vscode/launch.json:
"vmArgs": "-ea"


📁 Project Structure

ccrm/
 └── src/
     └── edu/ccrm/
         ├── cli/
         │   └── Main.java
         ├── domain/
         │   ├── Student.java
         │   ├── Instructor.java
         │   ├── Course.java
         │   ├── Grade.java
         ├── service/
         │   ├── StudentService.java
         │   ├── CourseService.java
         │   ├── EnrollmentService.java
         │   ├── BackupService.java
         │   └── ImportExportService.java
         └── util/
             └── DataStore.java


📦 Future Improvements


Move to JSON or database storage


Build a GUI-based desktop application


Enhance search & filtering






