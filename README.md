# Event Management API

A Django and Django REST Framework (DRF) based project for managing events. This API allows users to create, view, update, and delete events, manage participants, and handle authentication and permissions. Ideal for learning API development or building a real-world event management system.

---

## Features

- **User Authentication**: Registration, login, and JWT-based authentication.
- **Event Management**: Create, read, update, and delete events.
- **Permissions**: Only event creators can modify or delete their events.
- **RESTful APIs**: Easy-to-use endpoints.
- **Testing**: Unit tests for API endpoints.

---

## Technologies Used

- **Backend**: Django, Django REST Framework
- **Authentication**: JWT (JSON Web Token)
- **Database**: SQLite (default, can be changed to PostgreSQL/MySQL)
- **Testing**: Django test framework
- **Version Control**: Git

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/event_manager.git
   cd event_manager
Create and activate a virtual environment

bash
Copy code
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy code
pip install -r requirements.txt
Apply migrations

bash
Copy code
python manage.py migrate
Create a superuser (admin)

bash
Copy code
python manage.py createsuperuser
Run the server

bash
Copy code
python manage.py runserver
Access the API
Open your browser and go to http://127.0.0.1:8000/.

API Endpoints
Method	Endpoint	Description
GET	/api/events/	List all events
POST	/api/events/	Create a new event
GET	/api/events/<id>/	Retrieve event details
PUT	/api/events/<id>/	Update an event
DELETE	/api/events/<id>/	Delete an event
POST	/api/auth/register/	Register a new user
POST	/api/auth/login/	Login user and get JWT token

Running Tests
Run unit tests for the project using:

bash
Copy code
python manage.py test
Folder Structure
bash
Copy code
event_manager/
│
├── event_manager/      # Project settings
├── events/             # Event app
│   ├── migrations/
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── permissions.py
│   └── tests.py
├── manage.py
└── requirements.txt
Contributing
Fork the repository.

Create your feature branch (git checkout -b feature-name).

Commit your changes (git commit -m 'Add feature').

Push to the branch (git push origin feature-name).

Create a Pull Request.


