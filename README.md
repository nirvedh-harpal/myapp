# Library Token System

A Django-based web application for managing library compartments with student assignments and OTP-based deallocation.

## Features

- **User Authentication**: Separate login for students and security staff.
- **Student Dashboard**: Displays student's details and assigned compartment with OTP.
- **Security Dashboard**: Overview of all compartments, with options to assign and deallocate compartments.
- **Email Notifications**: Sends OTP and notifications via email to students.

## Technologies Used

- **Frontend**: HTML, CSS, Bootstrap
- **Backend**: Django
- **Database**: SQLite (for development)
- **Email**: Gmail SMTP
- **Deployment**: pythonanywhere

## Prerequisites

- Python 3.8 or higher
- Django 5.0.6

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/nirvedh-harpal/myapp.git
    cd library_token_system
    ```

2. **Create a virtual environment and activate it:**

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies:**

    ```sh
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**

    Create a `.env` file in the root directory and add the following:

    ```env
    SECRET_KEY=your-secret-key
    EMAIL_HOST_USER=your-email@gmail.com
    EMAIL_HOST_PASSWORD=your-email-password
    ```

5. **Run database migrations:**

    ```sh
    python manage.py migrate
    ```

6. **Create a superuser:**

    ```sh
    python manage.py createsuperuser
    ```

7. **Collect static files:**

    ```sh
    python manage.py collectstatic
    ```

8. **Run the development server:**

    ```sh
    python manage.py runserver
    ```

    The application will be available at `http://127.0.0.1:8000/`.

## Usage

- **Admin Panel**: Access the Django admin panel at `http://127.0.0.1:8000/admin/` to manage users, compartments, and other data.
- **Student Login**: Students can log in and view their dashboard at `http://127.0.0.1:8000/student_dashboard/`.
- **Security Login**: Security staff can log in and manage compartments at `http://127.0.0.1:8000/security_dashboard/`.

## Live Website

Check out the live application at [Library Token System](https://nirvedh.pythonanywhere.com/login/)

### Accessing the Student Dashboard

1. **Register**: Go to `https://nirvedh.pythonanywhere.com/register/` and create a new student account.
2. **Login**: After registration, log in with your new credentials at `https://nirvedh.pythonanywhere.com/login/`.
3. **Student Dashboard**: Once logged in, you will be redirected to the student dashboard at `https://nirvedh.pythonanywhere.com/student_dashboard/`.

### Accessing the Security Dashboard

1. **Login as Admin**: Use the following credentials to log in at `https://nirvedh.pythonanywhere.com/login/`:
   - **Username**: admin
   - **Password**: admin
2. **Security Dashboard**: Once logged in as an admin, you will be redirected to the security dashboard at `https://nirvedh.pythonanywhere.com/security_dashboard/`.

## Screenshots

### Login Page
![Login Page](images/login.png)

### Registration Page
![Registration Page](images/register.png)

### Student Dashboard
![Student Dashboard](images/student_dashboard.png)

### Security Dashboard
![Assign_Compartment](images/assign_compartment.png)
![Deallocate_Compartment](images/deallocate_compartment.png)

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any improvements or bug fixes.

## Contact

For any questions or support, please contact `harpalnirvedh@gmail.com`.



