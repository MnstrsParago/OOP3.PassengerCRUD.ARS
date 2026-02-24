# 🌐 Passenger CRUD REST API (ARS)

**Subject:** Object-Oriented Programming (OOP) / REST API / CRUD  
**Name:** Abdanur

## 📌 Project Description
This repository is a Java **REST API** for managing `Passenger` data in an Airline Reservation System (ARS).  
It supports **CRUD operations** (Create, Read, Update, Delete) and stores data in **PostgreSQL** using **JDBC**.

This project is a continuation of:
https://github.com/MnstrsParago/OOP2.HTTPServer.ARS

I used **Postman** to test all CRUD endpoints.

## 💡 Features
- Java HTTP server based REST API (`HttpServer`)
- CRUD endpoints for passengers:
  - `GET` all passengers
  - `POST` create a passenger
  - `PUT` update a passenger by id
  - `DELETE` remove a passenger by id
- JSON request/response handling
- PostgreSQL connection with JDBC
- Prepared statements to make SQL queries safer
- Easy testing with Postman

## 📦 Technologies
- **Java** (Java 17+ recommended)
- **PostgreSQL**
- **JDBC**
- **Java built-in HttpServer**
- **Postman** (for API testing)
- Git + GitHub

## 🚀 How to Run
1) Clone the repository:
```bash
git clone https://github.com/MnstrsParago/OOP3.PassengerCRUD.ARS.git
cd OOP3.PassengerCRUD.ARS
```

2) Make sure PostgreSQL is running, then create the table:
```sql
CREATE TABLE Passenger (
    passenger_id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    passport_number VARCHAR(50),
    nationality VARCHAR(50),
    date_of_birth DATE
);
```

3) Add required JAR files (if the project uses local libs in `lib/`):
- PostgreSQL JDBC driver
- JSON library (if used)

4) Update database settings in the code (URL / user / password).

5) Run `PassengerAPI.java`.

Server example:
```
http://localhost:8080/passenger
```

## 📘 Reflection
This project helped me understand how a simple REST API works in Java.  
I practiced handling HTTP requests, working with JSON, and connecting an API to a PostgreSQL database. Testing with Postman made it easy to verify that every CRUD operation works correctly.
