# Airbnb Clone Project

A full-stack clone of Airbnb to simulate a real-world booking platform.

## Project Goals
- Practice collaborative software development
- Understand backend and database design
- Implement secure APIs and CI/CD pipelines

## Tech Stack
- Django
- MySQL
- GraphQL
- Docker
- GitHub Actions

## Team Roles

- **Backend Developer**: Designs and implements backend APIs and handles logic.
- **Database Administrator (DBA)**: Designs schema, manages queries, ensures performance.
- **DevOps Engineer**: Manages CI/CD pipelines and deployment setup.
- **Security Analyst**: Implements API and system security protocols.
- **Project Manager**: Coordinates workflow, tracks progress, and manages tasks.

## Technology Stack

- **Django**: Backend web framework for building APIs and views.
- **MySQL**: Relational database to store users, bookings, and payments.
- **GraphQL**: API query language for flexible client-server communication.
- **Docker**: Containerization tool to ensure consistent environments.
- **GitHub Actions**: CI/CD tool to automate testing and deployment.

## Database Design

### Entities & Fields:

- **Users**: id, name, email, password, role
- **Properties**: id, owner_id (FK), title, location, price
- **Bookings**: id, user_id (FK), property_id (FK), start_date, end_date
- **Reviews**: id, user_id (FK), property_id (FK), rating, comment
- **Payments**: id, booking_id (FK), amount, status

### Relationships:

- One user can own many properties.
- A property can have many bookings and reviews.
- Each booking is linked to one user and one property.
- Each payment is tied to a booking.
