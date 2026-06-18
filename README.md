# Smart Food Delivery Management System

## Project Description

The Smart Food Delivery Management System is a backend application developed using FastAPI and MongoDB. The system provides RESTful APIs to manage restaurants, customers, menu items, orders, and payments in a food delivery platform.

The project demonstrates CRUD (Create, Read, Update, Delete) operations and database integration using MongoDB.

---

## Technologies Used

* Python 3
* FastAPI
* MongoDB
* MongoDB Compass
* PyMongo
* Pydantic
* Uvicorn

---

## Features

### Restaurant Management

* Add Restaurant
* View All Restaurants
* View Restaurant by ID
* Update Restaurant
* Delete Restaurant
* Search Restaurants by Location

### Customer Management

* Add Customer
* View All Customers
* View Customer by ID
* Update Customer
* Delete Customer

### Menu Management

* Add Menu Item
* View All Menu Items
* View Menu Item by ID
* Update Menu Item
* Delete Menu Item
* View Menu Items by Restaurant

### Order Management

* Create Order
* View All Orders
* View Order by ID
* Update Order
* Delete Order
* View Orders by Customer
* Update Order Status

### Payment Management

* Add Payment
* View All Payments
* View Payment by ID
* Update Payment
* Delete Payment

### Statistics Dashboard

* Total Restaurants
* Total Customers
* Total Menu Items
* Total Orders
* Total Payments

---

## Project Structure

SmartFoodDelivery/

├── database/

│   └── mongodb.py

├── models/

│   ├── restaurant.py

│   ├── customer.py

│   ├── menu_item.py

│   ├── order.py

│   └── payment.py

├── routes/

│   ├── restaurant_routes.py

│   ├── customer_routes.py

│   ├── menu_routes.py

│   ├── order_routes.py

│   └── payment_routes.py

├── main.py

├── requirements.txt

└── README.md

---

## Database

Database Name:

food_delivery_db

Collections:

* restaurants
* customers
* menu_items
* orders
* payments

---

## API Endpoints

### Restaurant APIs

* POST /restaurants
* GET /restaurants
* GET /restaurants/{restaurant_id}
* PUT /restaurants/{restaurant_id}
* DELETE /restaurants/{restaurant_id}
* GET /restaurants/location/{location}

### Customer APIs

* POST /customers
* GET /customers
* GET /customers/{customer_id}
* PUT /customers/{customer_id}
* DELETE /customers/{customer_id}

### Menu APIs

* POST /menu-items
* GET /menu-items
* GET /menu-items/{item_id}
* PUT /menu-items/{item_id}
* DELETE /menu-items/{item_id}
* GET /menu-items/restaurant/{restaurant_id}

### Order APIs

* POST /orders
* GET /orders
* GET /orders/{order_id}
* PUT /orders/{order_id}
* DELETE /orders/{order_id}
* GET /orders/customer/{customer_id}
* PUT /orders/{order_id}/status/{status}

### Payment APIs

* POST /payments
* GET /payments
* GET /payments/{payment_id}
* PUT /payments/{payment_id}
* DELETE /payments/{payment_id}

### Statistics API

* GET /stats

---

## How to Run the Project

### Step 1: Start MongoDB

Run MongoDB Server:

mongod --dbpath C:\data\db

### Step 2: Activate Virtual Environment

Windows:

venv\Scripts\activate

### Step 3: Install Dependencies

pip install -r requirements.txt

### Step 4: Run FastAPI Server

uvicorn main:app --reload

### Step 5: Open Swagger Documentation

http://127.0.0.1:8000/docs

---

## Testing

The APIs were tested using FastAPI Swagger UI and verified using MongoDB Compass.

---

## Future Enhancements

* User Authentication
* Admin Dashboard
* Delivery Partner Module
* Order Tracking System
* Review and Rating System
* Recommendation Engine

---

## Author

Nishtha Manish Wadaskar
24BCE10608
VIT Bhopal University
