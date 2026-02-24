# Fullstack-Bookstore-Epicbook

📘 EpicBook — Full‑Stack Bookstore Application
EpicBook is a full‑stack bookstore web application built using Node.js, Express, Handlebars, and Sequelize ORM, deployed on a Microsoft Azure Ubuntu VM with Nginx reverse proxy and Azure Database for MySQL.
The project follows a clean MVC architecture, supports CRUD operations for books and authors, includes cart and checkout functionality, and is fully production‑ready.

---

📑 Table of Contents

• 	Overview

• 	Features

• 	Tech Stack

• 	Project Structure

• 	Environment Variables

• 	Running Locally

• 	Database (Azure MySQL)

• 	Deployment on Azure VM

• 	Nginx Reverse Proxy Setup

• 	End‑to‑End Testing

• 	Common Issues

• 	Future Enhancements

---

🧾 Overview
EpicBook is a cloud‑deployed bookstore application that allows users to:
• 	Browse books
• 	View authors
• 	Add items to cart
• 	Checkout with address details
• 	Interact with a MySQL database hosted on Azure
The backend is powered by Node.js + Express, the frontend uses Handlebars templates, and the entire system is deployed on an Azure Ubuntu VM with Nginx acting as a reverse proxy.


---

⭐ Features
• 	Full CRUD for Books and Authors
• 	Shopping Cart system
• 	Checkout workflow
• 	Handlebars templating engine
• 	Sequelize ORM with MySQL
• 	Production deployment on Azure
• 	Reverse proxy with Nginx
• 	Auto‑created database tables

---


🛠️ Tech Stack
Frontend
• 	Handlebars (HBS)
• 	HTML5, CSS3, JavaScript
• 	Static assets served via Express
Backend
• 	Node.js
• 	Express.js
• 	Sequelize ORM
Database
• 	Azure Database for MySQL
Infrastructure
• 	Azure Ubuntu VM
• 	Nginx reverse proxy
• 	Systemd / manual Node process

📁 Project Structure
theepicbook/
│
├── server.js
├── .env
├── package.json
│
├── models/
│   ├── Author.js
│   ├── Book.js
│   ├── Cart.js
│   ├── Checkout.js
│   └── index.js
│
├── routes/
│   ├── bookRoutes.js
│   ├── authorRoutes.js
│   ├── cartRoutes.js
│   └── checkoutRoutes.js
│
├── views/
│   ├── layouts/
│   ├── partials/
│   ├── index.hbs
│   └── other templates...
│
└── public/
    ├── css/
    ├── js/
    └── images/

🔐 Environment Variables
Create a .env file:
DB_HOST=<azure-mysql-hostname>
DB_USER=<mysql-username>
DB_PASSWORD=<mysql-password>
DB_NAME=bookstore
PORT=8080

🧪 Running Locally
Install dependencies
npm install

Start the server
node server.js

Expected output
Executing (default): CREATE TABLE IF NOT EXISTS ...
App listening on PORT 8080

