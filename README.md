# Football Ticket Booking System Database

## Overview

This project is a database design and SQL assignment for a Football Ticket Booking System. The system manages football fans, football matches, and ticket bookings.

The project demonstrates:

* Database table design
* Primary Key and Foreign Key relationships
* Entity Relationship Diagram (ERD)
* SQL queries using JOINs, Subqueries, Aggregations, NULL handling, Pattern Matching, and Pagination

---

## Database Tables

### Users

Stores information about registered users and ticket managers.

Fields:

* user_id (Primary Key)
* full_name
* email
* role
* phone_number

### Matches

Stores football match information.

Fields:

* match_id (Primary Key)
* fixture
* tournament_category
* base_ticket_price
* match_status

### Bookings

Stores ticket booking records.

Fields:

* booking_id (Primary Key)
* user_id (Foreign Key)
* match_id (Foreign Key)
* seat_number
* payment_status
* total_cost

---

## Relationships

* One User → Many Bookings
* One Match → Many Bookings
* Each Booking belongs to one User and one Match

---

## SQL Concepts Used

* SELECT
* WHERE
* LIKE / ILIKE
* COALESCE
* INNER JOIN
* LEFT JOIN
* Aggregate Functions (AVG)
* Subqueries
* ORDER BY
* LIMIT
* OFFSET
* CHECK Constraints
* PRIMARY KEY
* FOREIGN KEY

---

## Assignment Queries

1. Retrieve available Champions League matches.
2. Search users by name using ILIKE.
3. Handle NULL payment status using COALESCE.
4. Display booking details with user and match information.
5. Display all users including users without bookings using LEFT JOIN.
6. Find bookings with total cost greater than the average booking cost.
7. Retrieve the top 2 most expensive matches while skipping the highest priced match.

---

## Files

* QUERY.sql — Database schema, sample data, and SQL queries.
* ERD.png — Entity Relationship Diagram.

---

## Author

Name: Razai Zim

Course Assignment: Football Ticket Booking System Database Design & SQL Queries
