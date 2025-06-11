# 🎬 Real-Time Cinema Management System

This repository contains the **Node.js Backend** for a full-featured **Real-Time Cinema Management Platform**.
It supports **multi-role access** (Admin, Vendor, Customer).

---

## 🔧 Technologies Used

* ⚙️ **Backend**: Node.js, Express.js, JWT
* 🛢️ **Database**: MongoDB
* 🧪 **Testing**: Postman
* 📡 **Communication**: REST API, WebSocket
* 🛡️ **Security**: JWT + Role-based Authorization
* 📧 **Email**: SMTP Integration
* 🔄 **Caching**: Redis

---

## 👥 System Roles & Features

### 👤 Admin

* Manages vendors: add, delete users, list vendors, and list customers
* Oversees cinema operations: views available movies and generates reports

### 👨‍🎬 Vendor

* Manages cinemas: adds, updates, deletes, and lists cinemas
* Handles halls: adds and lists halls
* Controls movies: adds, updates, deletes, and views available movies
* Manages showtimes: adds, updates, deletes, lists, and views seat maps

### 🍿 Customer

* Explores options: views available cinemas, last added movies, available movies, movie details, dates, showtimes, and seat maps
* Searches and filters: searches movies by title and applies filters
* Manages bookings: views bookings, user info, updates info, books seats, receives confirmation emails, and cancels bookings

---

## ⚙️ Node.js Backend Setup

### Prerequisites

* Node.js (v16 or higher)
* MongoDB running
* Redis server running
* SMTP credentials for emails
* JWT Secret configured

### Setup

```bash
# Clone the repository
git clone https://github.com/EhsanSamy/Real-Time-Cinema.git
cd Real-Time-Cinema

# Install Node.js dependencies
npm install

# Run the server
npm start
```

---

## 🔗 API Documentation

Test endpoints using Postman:
[http://localhost:3000/api](http://localhost:3000/api)

---

## 🗂️ Backend Folder Structure

```
├── app
│   ├── config
│   │   ├── auth.config.js
│   │   ├── db.config.js
│   │   └── email.config.js
│   ├── controllers
│   │   ├── admin.controller.js
│   │   ├── customer.controller.js
│   │   ├── user.controller.js
│   │   └── vendor.controller.js
│   ├── middlewares
│   │   ├── auth.controller.js
│   │   ├── authAdmin.js
│   │   ├── authCustomer.js
│   │   ├── authVendor.js
│   │   └── tokenblacklist.js
│   ├── models
│   │   ├── Bookings.js
│   │   ├── BookingSeats.js
│   │   ├── cinemas.js
│   │   ├── Halls.js
│   │   ├── index.js
│   │   ├── movies.js
│   │   ├── Reports.js
│   │   ├── seats.js
│   │   ├── Showtimes.js
│   │   └── users.js
│   ├── redis
│   │   └── redisClient.js
│   └── routes
│       ├── admin.routes.js
│       ├── customer.routes.js
│       ├── user.routes.js
│       └── vendor.routes.js
├── .env
├── app.js
├── package.json
└── server.js
```

---

## 🤝 Contribution

Feel free to **fork**, **improve**, and **submit pull requests**. Contributions are welcome!
