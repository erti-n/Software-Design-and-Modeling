# Software-Design-and-Modeling

SYSTEM ARCHITECTURE

- Student accesses the platform (Frontend)
- Frontend sends request to Backend (Django)
- Backend checks:
   Users table (authentication)
   Events table (event data)
   Registrations table (participation)
- Backend processes logic (filtering, validation, etc.)
- Backend returns data to Frontend
- Student registers → data stored in database

1- COMPONENT DIAGRAM (UML)

Components middle part:

Authentication Component: handles user login, registration, logout, and password checking.
Event Management Component: manages event creation, editing, deleting, listing, searching, and filtering.
Registration Component: handles student event registration, cancellation, and prevents duplicate registrations.
User Management Component: manages users, roles, and admin actions.

Notification Component: sends reminders and event update notifications to students.
Validation Service: checks if the entered data is correct before saving or processing it.
Authorization / Role Management: controls access based on user role, such as student, organizer, or admin.
Data Persistence Layer (ORM): reads and writes data from the database using Django ORM.
Database: Epoka EMS Database: stores users, events, and registrations.        

The diagram follows a three-tier architecture. The frontend sends requests to the Django backend components. The backend processes the requests using authentication, event management, registration, user management, and notification components. The ORM connects the backend with the database and handles reading and writing data.



