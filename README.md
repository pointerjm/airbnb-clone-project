
# Airbnb Clone Project

## Project Overview
The Airbnb Clone backend project provides a robust and scalable foundation for managing user interactions, property listings, bookings, payments, and reviews.  

### Project Goals
- Implement secure user registration, authentication, and profile management.  
- Enable property listing creation, updates, and retrieval.  
- Build a booking mechanism for users to reserve and manage bookings.  
- Integrate a payment system for processing transactions.  
- Allow users to leave reviews and ratings.  
- Ensure optimized performance with indexing and caching.  

### Tech Stack
- **Django** – Web framework for building APIs  
- **Django REST Framework** – Tools for RESTful endpoints  
- **PostgreSQL** – Relational database  
- **GraphQL** – Flexible querying for frontend  
- **Celery + Redis** – Asynchronous tasks and caching  
- **Docker** – Containerization for deployment  
- **GitHub Actions** – CI/CD automation


## Team Roles
- **Backend Developer**: Implements API endpoints, database schemas, and business logic.  
- **Database Administrator**: Designs and optimizes the database, manages indexes, and ensures data integrity.  
- **DevOps Engineer**: Handles deployment, scaling, CI/CD pipelines, and monitoring.  
- **QA Engineer**: Tests backend functionalities, ensures stability, and maintains quality standards.


## Technology Stack
- **Django**: High-level Python framework for backend APIs.  
- **Django REST Framework (DRF)**: RESTful API support.  
- **PostgreSQL**: Relational database for structured data.  
- **GraphQL**: Flexible and efficient query language.  
- **Celery**: Handles asynchronous tasks like notifications and payments.  
- **Redis**: Caching and session management.  
- **Docker**: Containerization for consistent environments.  
- **GitHub Actions**: Automates testing and deployment pipelines.


## Database Design
Key entities and fields:  

- **Users**: `id`, `name`, `email`, `password`  
- **Properties**: `id`, `owner_id`, `title`, `location`, `price`  
- **Bookings**: `id`, `property_id`, `user_id`, `start_date`, `end_date`  
- **Reviews**: `id`, `property_id`, `user_id`, `rating`, `comment`  
- **Payments**: `id`, `booking_id`, `amount`, `status`, `created_at`  

### Relationships
- A **User** can own multiple **Properties**.  
- A **Booking** belongs to a **Property** and is made by a **User**.  
- A **Review** is linked to both a **Property** and a **User**.  
- A **Payment** is tied to a **Booking**.
