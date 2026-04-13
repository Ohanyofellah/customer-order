# Customer Order API

A Django-based web application for managing customers and orders, featuring OpenID Connect (OIDC) authentication via Auth0, SMS notifications using Africa's Talking, and a responsive UI with Bootstrap. The project includes a REST API, unit tests, a CI/CD pipeline with GitHub Actions.

## Features
- **REST API**: Programmatically manage customers and orders.
- **Authentication**: Secure OIDC login/logout using Auth0.
- **SMS Notifications**: Send SMS alerts via Africa's Talking when new orders are created.
- **Responsive UI**: Built with Bootstrap 5, Google Fonts (Roboto), and custom CSS/JS with a sticky footer.
- **Testing**: Unit tests with coverage for core functionality.
- **CI/CD**: Automated testing and deployment via GitHub Actions and Heroku.

**Customer Order SetUp**
clone the repository and navigate to the project directory:
```bash
git clone 
cd customer-order
```                    
Make sure you have Python 3.11 installed, then

create a virtual environment and activate it:
```bashpython -m venv venv
source venv/bin/activate 
 # On Windows: v    env\Scripts\activate
 # On macOS/Linux: source venv/bin/activate
```     

To install pip and then all dependencies:
```bash
pip install --upgrade pip 
pip install -r requirements/base.txt

Create a .env file in the project root with the following content, replacing placeholders with your actual credentials:
```env
ask from the repository owner

Then outsource the .env file to set environment variables:
```bash
. env.sh

Then make the migrations and run the development server:
```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver