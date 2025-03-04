# Hotel Management System Database

## Overview
This project implements a relational database for a hotel management system. It includes tables for managing customers, bookings, reservations, rooms, staff, events, invoices, services, and financial transactions. The database ensures efficient data storage, retrieval, and integrity using SQL constraints and relationships.

## Database Schema
The database consists of the following tables:

- **customers**: Stores customer details like name, contact information, and address.
- **bookings**: Manages hotel room bookings, including check-in and check-out dates.
- **reservations**: Handles reservations with status tracking.
- **rooms**: Contains room details such as type, price, and availability.
- **staff**: Stores employee records, including roles and salaries.
- **events**: Manages event bookings within the hotel.
- **invoices**: Tracks billing and payments related to hotel stays and services.
- **services**: Stores details of additional hotel services provided to guests.
- **transactions**: Maintains financial transactions related to bookings, services, and payments.

## Features
- **Customer Management**: Stores customer information for easy access.
- **Booking System**: Enables reservations and room allocations.
- **Event Scheduling**: Allows event management within the hotel.
- **Invoice Generation**: Generates bills based on bookings and services.
- **Payment Tracking**: Records financial transactions for accountability.
- **Staff Management**: Maintains staff roles, salaries, and contact details.

## Setup Instructions
1. Install a database management system (MySQL, PostgreSQL, etc.).
2. Create a new database:  
   ```sql
   CREATE DATABASE hotel_management;
   ```
3. Use the database:  
   ```sql
   USE hotel_management;
   ```
4. Execute the SQL script to create tables and insert sample data.

## Usage
- Execute SQL queries to add, retrieve, update, or delete records.
- Perform joins to analyze customer booking trends.
- Generate financial reports by querying the `transactions` table.

## Example Queries
- Retrieve all active bookings:
  ```sql
  SELECT * FROM bookings WHERE status = 'active';
  ```
- List available rooms:
  ```sql
  SELECT * FROM rooms WHERE availability = 'available';
  ```
- Get total revenue:
  ```sql
  SELECT SUM(amount) FROM transactions WHERE type = 'payment';
  ```

## Future Improvements
- Implement stored procedures for common operations.
- Introduce triggers for automated updates.
- Develop a web interface for user-friendly management.

## License
This project is open-source and can be modified as needed.

---

**Author:** Syeda Mahroze Batool
**Date:** 4/March/2025

