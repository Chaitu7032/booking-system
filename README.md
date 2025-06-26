# Little Lemon Restaurant Booking App

This is a Django-based web application developed as part of a Coursera-guided project. The app allows customers to book restaurant tables by providing their first name, a reservation date, and a reservation slot (time). It features integration with a MySQL database and uses JavaScript (Fetch API) to display and update bookings dynamically.

## 🚀 Features

- 📅 Booking form with fields: First Name, Reservation Date, and Reservation Slot
- 🗓️ Date picker for selecting reservation date (HTML5 input type="date")
- ⏰ Time picker for selecting slot (HTML5 input type="time")
- 🔁 Fetch API used to get and refresh bookings without reloading the page
- 🛑 Prevents duplicate bookings on the same date and time slot
- 🧾 Displays all reservations for the selected date
- ❌ Shows "No Bookings" if no reservations exist for the chosen date
- ✅ Automatically selects today’s date on form load
- 📦 All bookings available as JSON through an API endpoint

## 🛠️ Tech Stack

- **Backend:** Django (Python)
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Environment Management:** Pipenv

## 📁 Project Structure

- `restaurant/` – Main Django app containing models, forms, views, and URLs
- `templates/booking_form.html` – Booking form and list display
- `static/js/fetch-bookings.js` – JavaScript for dynamic booking data

## 🧪 Setup Instructions

1. Create a pipenv environment and install dependencies:
   ```bash
   pipenv install django mysqlclient
   pipenv shell
   ```
2. Start Django project and app:
   ```bash
   django-admin startproject littlelemon .
   python manage.py startapp restaurant
   ```
3. Configure `settings.py` with MySQL credentials.
4. Apply migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
5. Run the server:
   ```bash
   python manage.py runserver
   ```

## 🤝 Acknowledgement

This project was developed under the guidance of Coursera's Django full-stack development course.

---

Feel free to clone, explore, or extend this project for your own learning or development use.
