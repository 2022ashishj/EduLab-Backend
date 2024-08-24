# EduLab-Backend

A simple and efficient backend API for managing users and tasks, designed to handle CRUD operations such as user registration, authentication, and task management.

## Installation

To set up and run this project locally, follow these steps:

1. Clone the repository:
   git clone <https://github.com/2022ashishj/EduLab-Backend.git>

2. Install the necessary dependencies:
   npm install

3. Start the server:
   npm start

4. API Endpoints

   -User Registration

   -Endpoint: /register

   -Method: POST

   -Request Body:
   {
   "username": "your username",
   "password": "password",
   "role":"user/admin"
   }

-response :("user registered successfully") 5. User Login

-Endpoint: /login

-Method: POST

-Request Body:
{
"username": "username",
"password": "password"
}

-Response:
("User logged in successfully")

7. Add Task

   -Endpoint: /tasks

   -Method: POST

   -Request Body:
   {
   "title": "Complete Project Documentation",
   "description": "Finish writing the project documentation and prepare it for review.",
   "status": "in-progress",
   "priority": "high",
   "assignedTo": "userObjectId", // Replace with the actual ObjectId of the assigned user
   "createdBy": "userObjectId" // Replace with the actual ObjectId of the user creating the task
   }

8. Get All Tasks

   -Endpoint: /tasks
   -Method: GET
   -Response: ("All tasks will appear in the response").

9. Get Filtered Tasks

   -Endpoint: /tasks/:id
   -Method: GET
   -Response: ("Filtered tasks based on query parameters will appear in the response.")

10. Delete Task

    -Endpoint: /tasks/:id
    -Method: DELETE
    -Response:
    ("Task deleted")

11. Deployment
    Deployed Link: [LINK](https://edulabs-backtemp.onrender.com)
