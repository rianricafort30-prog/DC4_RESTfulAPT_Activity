STUDENT RECORDS MANAGEMENT REST API (LARAVEL)

FILES INCLUDED:
- app/Models/Student.php
- app/Http/Controllers/StudentController.php
- routes/api.php
- database/migrations/2026_10_10_000000_create_students_table.php
- .env.example

HOW TO USE:
1. Create a Laravel project.
2. Copy each PHP file into the matching folder in your Laravel project.
3. Add the database details from .env.example to your .env file.
4. Create a MySQL database named student_records.
5. Run: php artisan migrate
6. Run: php artisan serve
7. Test the API at http://127.0.0.1:8000/api/students

API ENDPOINTS:
GET     /api/students       List students
POST    /api/students       Create a student
GET     /api/students/{id}  Show one student
PUT     /api/students/{id}  Update a student
DELETE  /api/students/{id}  Delete a student

POST/PUT JSON EXAMPLE:
{
  "student_id": "2026-001",
  "first_name": "Rian",
  "last_name": "Ricafort",
  "email": "rian@example.com",
  "course": "BSIT",
  "year_level": 3
}

NOTE: Keep the existing contents of your Laravel routes/api.php if it already has other routes; add the Route::apiResource line instead of overwriting everything.
