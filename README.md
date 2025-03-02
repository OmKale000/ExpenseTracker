# ExpenseTracker

ExpenseTracker is a Django-based web application for tracking personal expenses. This project has been set up using Django 3.0.5 and includes various modules and configurations to manage and monitor expenses effectively.

## Project Structure

The project is organized into the following main directories and files:

### ExpenseTracker/
Contains the main Django project settings and configurations.
- `__pycache__/`: Compiled Python files for performance optimization.
- `settings.py`: Django settings for the ExpenseTracker project.
- `urls.py`: URL routing configuration for the ExpenseTracker project.
- `wsgi.py`: WSGI configuration for deploying the Django application.

### home/
Contains the app for managing expenses.
- `migrations/`: Database migration files for the home app.
- `__pycache__/`: Compiled Python files for performance optimization.

## Getting Started

To get started with the ExpenseTracker project, follow these steps:

### Prerequisites

- Python 3.8+
- Django 3.0.5
- pip (Python package installer)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/OmKale000/ExpenseTracker.git
   cd ExpenseTracker
   ```

2. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```

### Running the Application

1. Apply database migrations:
   ```sh
   python manage.py migrate
   ```

2. Create a superuser to access the Django admin:
   ```sh
   python manage.py createsuperuser
   ```

3. Start the development server:
   ```sh
   python manage.py runserver
   ```

4. Open your web browser and navigate to `http://127.0.0.1:8000/` to access the application.

## Configuration

### Settings

The `settings.py` file contains various configuration options for the ExpenseTracker project. Key settings include:

- `DATABASES`: Configure your database settings here.
- `INSTALLED_APPS`: List of installed Django apps.
- `MIDDLEWARE`: Middleware settings for the project.
- `TEMPLATES`: Template settings for the project.
- `STATIC_URL`: URL for serving static files.

### Email Backend

The project is configured to send emails using the following settings in `settings.py`:
```python
EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'your_smtp_server'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = 'your_email@example.com'
EMAIL_HOST_PASSWORD = 'your_email_password'
```

Make sure to update these settings with your email server details.

## Deployment

To deploy the ExpenseTracker project to a production environment, follow the Django deployment checklist and configure your web server (e.g., Apache, Nginx) to serve the application using WSGI.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License.

## Acknowledgements

- Django Documentation: https://docs.djangoproject.com/en/3.0/
- Other resources and libraries used in this project.
