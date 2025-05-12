# CHAPTER ONE

## 1.1 Requirement Analysis (Use Case)

A high-level use case diagram for a kindergarten management system is a visual representation that provides a simplified overview of the system's core functionalities (use cases) and the primary roles (actors) that interact with it. It focuses on the main goals that different users can achieve through the system, without delving into the detailed steps or internal processes. It essentially paints a broad picture of what the system does and who interacts with it.

## 1.2 Components Of High-Level Use Case Diagram

### 1. Actors:
These are entities outside the system that interact with it. They represent roles that users or other systems can play. In your diagram, the actors are represented by stick figures and labeled:

- **Admin**: Represents the administrator of the KG Management System.
- **Teacher**: Represents the teachers who use the system.
- **Parent**: Represents the parents of the students.
- **System**: Represents an external system that interacts with the KG Management System (e.g., for payment processing or sending notifications).

### 2. Use Cases:
These represent the main functionalities or goals that the actors can achieve by interacting with the system. They are depicted as ovals and labeled with verb phrases indicating the action. Examples from your diagram include:

- Manage User Accounts
- Authenticate User
- Manage System Settings
- Manage Class Information
- Make Payments
- Process Payment
- Manage Classes
- Record Student Attendance
- Communicate with Parents
- Manage Learning Materials
- Send Notifications
- Communicate with Teacher
- Manage Child Profile
- View Progress Reports

### 3. System Boundary:
This is the rectangle that encloses all the use cases. It visually defines the scope of the KG Management System, separating it from the external actors. The label "KG Management System" at the top of the rectangle clearly identifies what the system is.

### 4. Relationships:
These illustrate how actors interact with use cases and how use cases relate to each other. The types of relationships shown in your diagram are:

- **Association**: Represented by a solid line connecting an actor to a use case. It indicates that the actor participates in or initiates that use case. For example, the Admin is associated with "Manage User Accounts" and "Manage System Settings."

- **Include (`<<include>>`)**: Represented by a dashed arrow with an open arrowhead pointing from a base use case to an included use case, labeled with `<<include>>`. It signifies that the base use case explicitly incorporates the behavior of the included use case. For example, "Manage User Accounts" `<<include>>` "Authenticate User", meaning that authenticating a user is a necessary step within managing user accounts. Similarly, "Make Payments" `<<include>>` "Process Payment".

- **Extend (`<<extend>>`)**: Represented by a dashed arrow with an open arrowhead pointing from an extending use case to a base use case, labeled with `<<extend>>`. It indicates that the extending use case provides additional or optional behavior to the base use case at specific extension points. For example, "Send Notifications" `<<extend>>` "Communicate with Parents," suggesting that sending notifications is an optional extension of the communication process. Similarly, "View Progress Reports" `<<extend>>` "Manage Child Profile" with an extension point "upload child info," and "Communicate with Teacher" and "Communicate with Parents" are extended by the possibility of sending attachments.

## 1.3 Example Of High-Level Use Case Diagram

*(Insert your use case diagram image here)*

**Figure 1.1** High-Level Use Case Diagram for Kindergarten Management

## 1.4 Overall Description of the KG Management System Use Case Diagram

### Actors:

- **Parent**: Interacts with the system for tasks like student registration, receiving notifications, communicating with teachers, viewing the event calendar and fee statements, making payments, viewing course details, and managing their login (resetting password).

- **Teacher**: Interacts with the system for login, viewing student information, recording student progress, submitting reports, communicating with parents, managing classroom activities, enrolling students in classes, viewing the classroom schedule, and marking attendance.

- **Administrator**: Has comprehensive access for managing the system, including registering new users, reviewing user registrations, assigning and revoking roles, managing permissions, student records, teacher records, and attendance records. They also handle financial aspects like verifying payments and generating reports, as well as scheduling events and managing their login (including password recovery and logout).

- **TeleBirr**: Represents an external payment gateway system that interacts with the Kindergarten Management System for processing payments and generating receipts.

### Key Use Cases:

The diagram illustrates a wide range of functionalities, broadly categorized as:

- **User Management**: Registration, Login, Logout, Reset Password, Recover Password, Review User Registration, Assign/Revoke Role, Manage Permissions.

- **Student Management**: Make Student Registration, View Student Information, Record Student Progress, Enroll Class, View Classroom Schedule, Manage Student Records, Mark Attendance, Manage Attendance Records.

- **Communication**: Receive Notification, Communicate with Teacher, Communicate with Parent, View Event Calendar.

- **Financial Management**: View Fee Statement, Make Payment, Verify Payment, Process Payment, Generate Receipt.

- **Course/Class Management**: View Course Detail, Manage Classroom Activities.

- **Reporting**: Submit Report, Manage Teacher Records, Schedule Events.

### Relationships:

- **Associations**: Solid lines connect actors to the use cases they participate in.
- **`<<include>>`**: Dashed arrows labeled `<<include>>` indicate that a base use case incorporates the behavior of another use case. For example, "Make Student Registration" includes "Receive Notification".
- **`<<extend>>`**: Dashed arrows labeled `<<extend>>` indicate that an extending use case adds optional behavior to a base use case at a specific extension point. For example, "Reset Password", "Recover Password", and "Logout" extend the "Login" use case at the extension points of Login.
