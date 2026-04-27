# To-Do List API

A simple and clean REST API built with FastAPI and SQLite to manage daily tasks.

## Tech Stack

- Python 3.x
- FastAPI
- SQLAlchemy
- SQLite
- Uvicorn

## Features

- Create tasks with title and description
- View all tasks or a single task
- Update task details and mark as completed
- Delete tasks
- Auto-generated Swagger UI documentation

## Project Structure

todo_api/
├── main.py         # API routes and logic
├── database.py     # Database connection setup
├── models.py       # Database models
└── requirements.txt

## Installation & Setup

1. Clone the repository
   git clone https://github.com/Dhanush1728/todo-api.git
   cd todo-api

2. Install dependencies
   pip install -r requirements.txt

3. Run the server
   uvicorn main:app --reload

4. Open Swagger UI
   https://to-do-list-api-fbl1.onrender.com/docs

## API Endpoints

| Method | Endpoint        | Description          |
|--------|-----------------|----------------------|
| GET    | /tasks          | Get all tasks        |
| GET    | /tasks/{id}     | Get a single task    |
| POST   | /tasks          | Create a new task    |
| PUT    | /tasks/{id}     | Update a task        |
| DELETE | /tasks/{id}     | Delete a task        |

## Sample Request

POST /tasks
{
  "title": "Buy groceries",
  "description": "Milk, eggs, bread"
}

## Sample Response

{
  "id": 1,
  "title": "Buy groceries",
  "description": "Milk, eggs, bread",
  "completed": false
}

## Author

Your Name
GitHub: github.com/Dhanush1728
