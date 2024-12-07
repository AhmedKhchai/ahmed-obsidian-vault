- Option 1: Keep the permissions loose until LMS features are implemented.
- Option 2: setup permission only for admins.

```
erDiagram
    School {
        integer id PK
        string name
        string address
        string phone
        string email
        string logo
        User users
        Group groups
        Subject subjects
        Course courses
        Teacher teachers
        Student students
        Payment payments
        Discount discounts
    }
```


```
erDiagram
    Role {
        integer id PK
        string name
    }
    Permission {
        integer id PK
        string name
    }
    UserRole {
        integer user_id FK
        integer role_id FK
    }
    RolePermission {
        integer role_id FK
        integer permission_id FK
    }
```

Creating a **sober and effective set of default user permissions and roles** for a School Management System with Learning Management System functionalities involves establishing clear distinctions between the capabilities of superadmins, admins, teachers, and students. Below is a suggested setup for these roles and their respective permissions. This setup assumes the use of a role-based access control (**RBAC**) system, where permissions can be assigned directly to roles and users can be assigned one or more roles.

### Roles

1. **Superadmin**: Has overarching access to the entire system. Can manage schools, admins, system-wide settings, and all data.
2. **Admin**: Manages school-level configurations, users (teachers and students), courses, schedules, and reports within their school.

### Permissions

#### Superadmin Permissions

- Manage schools: Create, update, delete schools.
- Manage system settings: Update system-wide configurations and settings.
- Manage all users: Create, update, delete any user in the system.
- View all data: Access to all data across schools for monitoring and analytics.

#### Admin Permissions

- Manage users: Create, update, delete teachers and students (other school related entities ex: Discounts, Groups, Subjects, Courses, Attendance....) within their school.
- Manage school: Create, update, delete courses, subjects, and groups within their school.
- Configure school settings: Update settings specific to their school, like logo, contact info, etc.

#### Teacher Permissions

- Manage course content: Add, update, delete course materials, assignments, quizzes.
- Grade assignments: Review and grade student submissions.
- Communicate with students: Send announcements, answer questions, and facilitate discussions.
- View student progress: Monitor student performance and engagement in their courses.

#### Student Permissions

- Access course content: View course materials, assignments, quizzes.
- Submit assignments: Upload or complete assignments online.
- View grades: Check grades for assignments and overall course performance.
- Participate in discussions: Engage in course discussions and communicate with teachers and peers.