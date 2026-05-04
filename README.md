# Software-Design-and-Modeling

SYSTEM ARCHITECTURE

- Student accesses the platform (Frontend)
- Frontend sends request to Backend (Django)
- Backend checks:
   - Users table (authentication)
   - Events table (event data)
   - Registrations table (participation)
- Backend processes logic (filtering, validation, etc.)
- Backend returns data to Frontend
- Student registers → data stored in database
