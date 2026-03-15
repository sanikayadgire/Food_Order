# Food Ordering Web Application

## Overview

This project is a web based food ordering system. Users can browse food items, add them to a cart, and place orders online. The system also includes an admin panel that allows administrators to manage food items, orders, and users.

The project demonstrates basic full stack web development using PHP, MySQL, HTML, CSS, and JavaScript. It implements user authentication, cart management, order processing, and administrative control.

This project is useful for learning database driven web applications and CRUD operations.

---

## Features

### User Features

* User registration and login
* Browse food categories
* View food items with images and prices
* Add food items to cart
* Update or remove items from cart
* Checkout and place orders
* View previous orders

### Admin Features

* Admin login authentication
* Admin dashboard
* Add new food items
* Update food item details
* Delete food items
* View and manage customer orders
* Manage admin accounts

---

## Technology Stack

### Frontend

* HTML
* CSS
* JavaScript

### Backend

* PHP

### Database

* MySQL

### Server

* Apache (XAMPP / WAMP / LAMP)

---

## Project Structure

```
Food_Order/

│
├── admin/
│   Admin dashboard and management pages
│
├── components/
│   Contains reusable PHP components such as:
│   - database connection
│   - header and footer
│   - common functions
│
├── css/
│   Stylesheets for frontend and admin panel
│
├── js/
│   JavaScript files for UI interaction
│
├── images/
│   Static images used in the website
│
├── uploaded_img/
│   Images uploaded for food items
│
├── index.php
│   Homepage of the application
│
├── menu.php
│   Displays available food items
│
├── cart.php
│   Shopping cart functionality
│
├── checkout.php
│   Handles order checkout process
│
├── orders.php
│   Displays user order history
│
├── login.php
│   User login page
│
├── register.php
│   User registration page
│
└── about.php / contact.php
    Additional informational pages
```

---

## Database Setup

Database Name

```
food_db
```

Steps to setup database

1. Start **Apache** and **MySQL** using XAMPP.
2. Open **phpMyAdmin**.
3. Create a new database.

```
food_db
```

4. Import the provided SQL file into the database.

---

## Database Configuration

Database connection file location

```
components/connect.php
```

Default configuration

```
Host: localhost
Username: root
Password: (empty)
Database: food_db
```

Modify these values if your MySQL credentials are different.

---

## Installation Guide

Step 1
Install **XAMPP** or any PHP server environment.

Step 2
Copy the project folder into the `htdocs` directory.

Example

```
C:/xampp/htdocs/Food_Order
```

Step 3
Start the following services from XAMPP control panel

* Apache
* MySQL

Step 4
Import the database using phpMyAdmin.

Step 5
Open the project in your browser.

```
http://localhost/Food_Order
```

---

## Admin Panel Access

Admin login page

```
http://localhost/Food_Order/admin/admin_login.php
```

The admin panel allows administrators to:

* manage food products
* monitor orders
* manage users and admins

---

## Core Modules

### Authentication Module

Handles user registration and login using PHP sessions.

### Product Module

Displays food items stored in the database.

### Cart Module

Manages cart operations such as adding, updating, and removing items.

### Order Module

Processes user orders and stores order details in the database.

### Admin Management Module

Provides administrative control over products and orders.

---

## Security Considerations

Current implementation is basic and requires improvements for production use.

Issues

* Passwords may not use secure hashing
* Limited input validation
* SQL injection protection should be improved

Recommended improvements

* Use `password_hash()` and `password_verify()`
* Use prepared statements
* Implement input validation and sanitization
* Add CSRF protection

---

## Future Improvements

* Payment gateway integration
* Order tracking system
* Search and filtering of food items
* Email notifications
* REST API support
* Mobile responsive UI
* Docker deployment
* Modern frontend framework integration

---

## Learning Outcomes

This project demonstrates

* CRUD operations using PHP and MySQL
* Session based authentication
* Database driven dynamic web pages
* Shopping cart logic
* Admin panel implementation
* Basic e-commerce workflow

---

## License

This project is created for educational purposes.
