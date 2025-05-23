# README.md for Django Quiz API Project

## Project: Django Quiz API

### Description
This project is a RESTful API built using Django and Django REST Framework to manage quizzes, questions, choices, and user profiles. The API supports CRUD operations and includes endpoints for user authentication, quiz creation, and validation of quiz answers.

### Features
- User profile management
- Quiz creation and retrieval
- Question and choice association
- Quiz answer validation
- Media support for profile avatars
- User authentication and profile linking

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Francys999/lab08_dae
   ```

2. Navigate to the project directory:
   ```bash
   cd django-quiz-api
   ```

3. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

5. Apply migrations:
   ```bash
   python manage.py migrate
   ```

6. Run the server:
   ```bash
   python manage.py runserver
   ```

### API Endpoints
- **/api/quizzes/**: List and create quizzes
- **/api/questions/**: List and create questions
- **/api/choices/**: List and create choices
- **/api/users/profiles/**: User profile management
- **/api/quizzes/{id}/validate/**: Validate answers for a specific quiz

### Testing
To test the API, use Thunder Client or Postman. Example:
```bash
curl -X POST http://127.0.0.1:8000/api/quizzes/ -d '{"title": "Python Basics", "description": "Basic Python questions"}'
```

### License
MIT License