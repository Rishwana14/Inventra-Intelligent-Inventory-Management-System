Inventra – Intelligent Inventory Management System
1. Overview

Inventra is a full-stack intelligent inventory management system designed to provide real-time stock tracking, automated low-stock alerts, and efficient transaction handling. The system integrates a React frontend, Java backend, and MySQL database to ensure reliable, scalable, and structured inventory control for retail and warehouse environments.

The platform minimizes manual errors, improves stock visibility, and supports informed restocking decisions.

2. Problem Statement

Many small and medium businesses rely on manual or semi-digital methods to track inventory. These approaches lead to:

Inaccurate stock levels

Delayed identification of low inventory

Overstocking and financial loss

Lack of centralized transaction records

Inventra solves these problems through automation, centralized data storage, and rule-based alert mechanisms.

3. System Architecture

The system follows a three-tier architecture:

3.1 Frontend Layer (Client Side)

Built using React, this layer provides:

Interactive dashboard

Product management interface

Transaction entry forms

Alert display panel

3.2 Backend Layer (Application Server)

Built using Java (Spring Boot recommended):

RESTful API services

Business logic for inventory updates

Alert generation logic

Authentication and authorization

3.3 Database Layer

MySQL is used for persistent storage:

Product records

Stock quantities

Transaction history

User accounts

Alert logs

4. Key Features
4.1 Authentication & Authorization

Secure login system

Role-based access control (Admin / Manager)

4.2 Product Management

Add new products

Update product details

Delete obsolete items

Maintain stock and pricing information

4.3 Real-Time Stock Tracking

Automatic stock updates after each transaction

Prevents negative stock entries

4.4 Intelligent Alert System

Detects when stock falls below threshold

Generates low-stock alerts for timely restocking

4.5 Transaction Management

Records purchase and sales transactions

Maintains detailed transaction history

Tracks stock inflow and outflow

4.6 Dashboard & Insights

Displays inventory summary

Highlights low-stock products

Provides quick operational insights

5. Technology Stack
Layer	Technology
Frontend	React.js, HTML, CSS, JavaScript
Backend	Java, Spring Boot, REST APIs
Database	MySQL
Version Control	Git, GitHub
6. Module Description
Module 1 – Authentication Module

Handles secure login, user sessions, and role-based access control.

Module 2 – Product Management Module

Manages product catalog, pricing, suppliers, and stock levels.

Module 3 – Alert Module

Continuously monitors stock levels and generates alerts when thresholds are breached.

Module 4 – Transaction Module

Processes sales and purchase transactions and updates inventory automatically.

7. Database Design (High-Level Schema)

Tables include:

Users (user_id, username, password, role)

Products (product_id, name, category, price, stock_quantity, threshold)

Suppliers (supplier_id, name, contact_info)

Transactions (transaction_id, product_id, type, quantity, date)

Alerts (alert_id, product_id, message, status, created_at)

8. Installation & Setup
8.1 Clone Repository
git clone https://github.com/YOUR-USERNAME/Inventra-Intelligent-Inventory-Management-System.git
cd Inventra-Intelligent-Inventory-Management-System

8.2 Backend Setup (Java)

Open backend folder in IDE (IntelliJ / Eclipse)

Configure application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/inventra_db
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update


Run the Spring Boot application

Server runs on:

http://localhost:8080

8.3 Frontend Setup (React)
cd frontend
npm install
npm start


Frontend runs on:

http://localhost:3000

8.4 Database Setup (MySQL)

Create database:

CREATE DATABASE inventra_db;


Import schema (if SQL file provided)

9. API Communication

The React frontend communicates with the Java backend using REST APIs.

Example endpoints:

Method	Endpoint	Description
GET	/api/products	Fetch all products
POST	/api/products	Add new product
PUT	/api/products/{id}	Update product
DELETE	/api/products/{id}	Delete product
POST	/api/transactions	Record transaction
GET	/api/alerts	Fetch low-stock alerts
10. Future Enhancements

AI-based demand forecasting

Barcode and QR code integration

Supplier performance tracking

Cloud deployment

Mobile application support

11. Contributors

Developed as a team project under the title
Inventra – Intelligent Inventory Management System
team members- Rishwana Sirajutheen,Dritisai sivarathri,Naga Syamala Chintapalli,Tanoor Kiran,Hemanth Raava
