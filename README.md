# airbnb-clone-project

## Project Overview
This project is a clone of the the AirBnB project for the pro backend course ofn ALX. The goal of this project is to enhance expertise in modern software development practices. The learner will learn about:
1. Github Repository Management
2. Team Role Documentation
3. Tech Stack Breakdown
4. Databbase Design
5. Feature-Driven Development
6. API Security Fundamentals
7. CI/CD Pipeline Integration

### Tech Stack includes;
1. Github
2. Django
3. MySQL
4. GraphQL

## Team Roles

### Backend Developer
Handles the server-side logic and API development using Django.

### Frontend Developer
Builds the user interface using HTML/CSS/JS or React.

### Database Administrator (DBA)
Designs and optimizes PostgreSQL database structures.

### DevOps Engineer
Manages containerization, deployment, and CI/CD pipelines.

### Project Manager
Coordinates task management, timelines, and progress tracking.

## Technology Stack

- **Django**: Web framework for backend development.
- **PostgreSQL**: Relational database to store structured data.
- **GraphQL**: Query language for efficient API data fetching.
- **Docker**: Used for containerizing the app and running consistent environments.
- **React (Optional)**: Library for building interactive UIs on the frontend.

## Database Design

### Entities and Fields

**1. Users**
- id
- name
- email
- password
- role

**2. Properties**
- id
- user_id (FK)
- title
- description
- price_per_night

**3. Bookings**
- id
- user_id (FK)
- property_id (FK)
- start_date
- end_date

**4. Reviews**
- id
- user_id (FK)
- property_id (FK)
- rating
- comment

**5. Payments**
- id
- booking_id (FK)
- amount
- payment_method
- status

### Relationships
- A **User** can own multiple **Properties**
- A **Property** can have multiple **Bookings** and **Reviews**
- A **Booking** links a **User** to a **Property**
- A **Review** is written by a **User** for a **Property**
- A **Payment** is linked to a **Booking**