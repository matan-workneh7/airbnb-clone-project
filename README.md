# Airbnb Clone Project

## Overview
The Airbnb Clone Project dives deep into full-stack development, enabling learners to understand the complex architecture and workflows of building a robust, real-world booking platform like Airbnb.

## Project Goals
- Master collaborative team workflows using GitHub  
- Deepen understanding of backend architecture and database design principles  
- Implement advanced security measures for API development  
- Gain proficiency in designing and managing CI/CD pipelines for efficient deployment  
- Strengthen the ability to document and plan complex software projects effectively  
- Develop an understanding of integrating technologies like Django, MySQL, and GraphQL in a unified ecosystem  

## Technology Stack
- **Backend Framework:** Django - for providing developers with pre-built code, tools, and structures for building the server-side
- **Database:** MySQL  - for providing a structured and efficient way to organize information within a database. 
- **API Layer:** GraphQL  - for allowing clients to request specific data from an API, rather than receiving a predefined set of data. 
- **Containerization:** Docker  - for simplifying the process of building, deploying, and running applications using containers.
- **CI/CD:** GitHub Actions  - for automating software development workflows within your GitHub repositories.

## Team Roles

### Backend Developer
Focuses on building the server-side logic, APIs, and integrating with databases. Responsible for ensuring code quality, scalability, and security.  

### Database Administrator (DBA)
Manages database design, optimization, and maintenance. Ensures data integrity, performance, and backups are in place.  

### Frontend Developer
Builds the user interface and ensures smooth user experience. Responsible for integrating frontend components with backend APIs.  

### DevOps Engineer
Sets up and maintains CI/CD pipelines, containerization, and cloud infrastructure. Responsible for monitoring system reliability and deployments.  

### Project Manager
Coordinates tasks, timelines, and communication across the team. Ensures project goals and deadlines are met.  

### QA Engineer
Tests features and validates functionality. Ensures the application is bug-free, reliable, and secure before release.  

## Database Design

### Users
- Fields: id, name, email, password, role  
- A user can own multiple properties and make multiple bookings.  

### Properties
- Fields: id, title, description, location, price_per_night  
- Each property belongs to one user (the host).  
- A property can have many bookings and many reviews.  

### Bookings
- Fields: id, user_id, property_id, start_date, end_date, status  
- A booking belongs to one user and one property.  

### Payments
- Fields: id, booking_id, amount, status, payment_date  
- Each payment is linked to one booking.  

### Reviews
- Fields: id, user_id, property_id, rating, comment  
- A review is made by a user for a property.  

