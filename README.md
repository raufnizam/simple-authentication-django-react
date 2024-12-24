# MyApp: Login, Registration, and User Dashboard

A fully functional web application built using **Django REST Framework (DRF)** for the backend and **React** (with Vite) for the frontend. The app features user authentication with JWT tokens, a registration system, and a user dashboard displaying profile information.

---

## Features

- User Registration
- User Login with JWT Authentication
- Responsive Navbar
- Protected User Dashboard with Profile Information
- Tailwind CSS for modern styling

---

## Tech Stack

- **Backend:** Django REST Framework (DRF)
- **Frontend:** React (Vite) with Tailwind CSS
- **Authentication:** JWT (via `djangorestframework-simplejwt`)
- **API Communication:** Axios

---

## Prerequisites

- Node.js (>=16.x)
- Python (>=3.8)
- Django (>=3.2)
- Vite

---

## Installation and Setup

### Backend Setup (Django)

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/myapp.git
   cd myapp/backend
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/Mac
   venv\Scripts\activate   # For Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Apply migrations and run the server:
   ```bash
   python manage.py migrate
   python manage.py runserver
   ```

The backend will be available at `http://127.0.0.1:8000/`.

### Frontend Setup (React)

1. Navigate to the `frontend` directory:
   ```bash
   cd ../frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will be available at `http://127.0.0.1:5173/`.

---

## Usage

1. **Register a new user**: Visit `http://127.0.0.1:5173/register` to create an account.
2. **Login**: Go to `http://127.0.0.1:5173/login` to log in.
3. **Dashboard**: After logging in, visit `http://127.0.0.1:5173/dashboard` to view the user's profile.
4. **Logout**: Use the Logout button in the Navbar to log out.

---

## Project Structure

```
myapp/
├── backend/                # Django backend
│   ├── auth_app/           # Authentication app
│   ├── manage.py           # Django management script
│   └── requirements.txt    # Backend dependencies
├── frontend/               # React frontend
│   ├── src/
│   │   ├── components/     # React components (Navbar, Login, Register, Dashboard)
│   │   ├── App.jsx         # Main React App
│   │   └── index.css       # Tailwind CSS setup
│   └── package.json        # Frontend dependencies
└── README.md               # Project documentation
```

---

## API Endpoints

### Authentication

- **POST** `/auth/register/`: User registration
- **POST** `/auth/login/`: User login with JWT tokens
- **GET** `/auth/profile/`: Fetch the logged-in user's details (requires token)

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
