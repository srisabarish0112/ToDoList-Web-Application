# TodoList App

## **Overview**

This is a simple TodoList web application built with Django, Django REST Framework (DRF), and SQLite. The app allows users to create, update, and delete tasks, providing an easy way to manage daily to-do lists. 

### **Features**
- **User Authentication**: Login and register to manage your tasks securely.
- **Task Management**: Add,delete and mark tasks as completed.
- **REST API**: A RESTful API for managing tasks.
- **SQLite Database**: All user data and tasks are stored in a lightweight SQLite database.

---

## **Technologies Used**

- **Django**: Web framework for building the application.
- **Django REST Framework (DRF)**: For creating the RESTful API.
- **SQLite Database**: Lightweight database for storing user data and tasks.
- **Frontend**: HTML, CSS, and JavaScript for the user interface.

---

## **Procedure**

### 1. **Set Up the Environment**
   - Install Python and Django:
     ```bash
     pip install django
     pip install djangorestframework
     ```
   - Create a Django project and a Todo app within the project.
   - Set up the SQLite database by running the migrations:
     ```bash
     python manage.py migrate
     ```

### 2. **User Authentication**
   - Implemented login and registration functionality using Django's built-in authentication system.
   - Users can register an account and log in to manage their tasks securely.

### 3. **Task Management**
   - Users can add, edit, and delete tasks. 
   - Each task has a name and description and is stored in the SQLite database.

### 4. **REST API**
   - Created a REST API to interact with tasks.
   - The API allows users to view, create, update, and delete tasks using HTTP requests (GET, POST, PUT, DELETE).
   
### 5. **Frontend Interface**
   - Used HTML/CSS for designing the UI to display login and task management interfaces.
   - JavaScript was used for front-end logic to interact with the backend API.

---

## **Usage**

### 1. **Login Interface**
   - After running the app, you will be prompted to log in using your registered credentials.
   - If you don’t have an account, you can register by clicking the register link on the login page.

   ![Login Interface](https://github.com/user-attachments/assets/8ff36d5f-a80b-42ef-a53e-9c981447d1e0)

### 2. **Task Adding Interface**
   - Once logged in, you can add a new task by providing a task name and description.
   - The new task will be saved to the SQLite database and displayed in the task list.

   ![Task Adding Interface](https://github.com/user-attachments/assets/670123e5-2862-48c8-bdf6-34736006fc11)

### 3. **REST API**
   - The application exposes a REST API that allows users to manage tasks programmatically.
   - Example API endpoints:
     - `GET /api/tasks/` - View all tasks.
     - `POST /api/tasks/` - Add a new task.
     - `PUT /api/tasks/{id}/` - Update a task.
     - `DELETE /api/tasks/{id}/` - Delete a task.

---

## **Installation**

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/todolist-app.git
   cd todolist-app
