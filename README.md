Laptop Management System
This system can be used by organizations to manage their inventory of laptops, track
assignments to employees, and schedule maintenance.
Project Features
User Roles
1. Admin: Manage laptops, assign laptops to employees, track status, and view
reports.
2. Employee: View assigned laptops, request new laptops, or report issues.
Core Features
● Laptop inventory management (add, update, delete laptops).
● Laptop assignment to employees.
● Maintenance tracking and history.
● Reporting issues (with status updates).
● Filters and search functionality (by employee, laptop status, or maintenance status).
Frontend Tasks
1. Admin Dashboard:
○ Overview cards for:
■ Total laptops.
■ Assigned laptops.
■ Available laptops.
■ Laptops under maintenance.
○ Manage Laptops:
■ Add a new laptop with details (e.g., brand, model, serial number,
purchase date).
■ Update or delete existing laptops.
○ Employee Assignment:
■ Assign laptops to employees (search employees by name/email).
■ Reassign or unassign laptops.
■
2.Employee Portal:
● View assigned laptop details (brand, model, serial number, condition).
● Request a new laptop (form submission).
● Report an issue (with description and priority level).

Backend Tasks
1. APIs for Laptop Management:
○ Add a laptop:
○ Get all laptops:
○ Update laptop details:
○ Delete a laptop:
2. APIs for Employee Management:
○ Get all employees:
○ Assign a laptop:
○ Fetch laptops assigned to an employee:
3. APIs for Maintenance and Issue Reporting:
○ Add a maintenance log:
○ View maintenance history:
○ Report an issue:
4. Database Schema:
○ Tables:
■ laptops: id, brand, model, serialNumber, status
(available/assigned/maintenance), purchaseDate.
■ employees: id, name, email, department.
■ assignments: id, laptopId, employeeId, assignedAt, returnedAt.
■ maintenance: id, laptopId, description, status, cost, loggedAt.
■ issues: id, laptopId, description, priority, status, reportedBy,
reportedAt.
5. Authentication:
○ Implement JWT-based authentication.
○ Ensure role-based access control (Admin vs. Employee).

Evaluation Criteria
● Code Quality: Clean code with proper modularity and comments.
● Functionality: All CRUD operations and role-based workflows should be
implemented.
● UI/UX: Intuitive and responsive interface.
● Backend Performance: Proper database indexing and efficient queries.
