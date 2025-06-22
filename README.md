# airbnb-clone-project
The Airbnb Clone Project is a full-stack web application inspired by the popular booking platform, Airbnb. This project is designed to simulate the development of a real-world, scalable web app with complex features such as user authentication, property listing, booking management, secure payment handling, and interactive UI/UX.
Through this project, learners gain hands-on experience in backend systems, database schema design, RESTful API development, authentication/authorization, and secure application deployment. It also emphasizes real-world software engineering practices such as team collaboration, version control, and modular design.

# Team Roles
Backend Developer is responsible for designing and implementing RESTful API endpoints that support key functionalities such as user registration, property listing, bookings, and reviews. They also enforce business logic to maintain data integrity and proper user permissions, collaborate closely with frontend developers to ensure smooth API integration, and write clean, modular code that supports scalability and long-term maintenance.

Database Administrator (DBA) handles the database design and schema structure to efficiently store user data, property listings, bookings, and transactions. Their responsibilities include optimizing query performance through indexing, monitoring database usage and security, and maintaining regular backups to support disaster recovery.

DevOps Engineer manages the deployment process and system infrastructure. They set up and maintain CI/CD pipelines to automate build and deployment workflows, configure cloud services like AWS, Azure, or DigitalOcean to host the backend, monitor server health and logs to prevent downtime, and utilize Docker for containerization to streamline environment setup and scalability.

QA Engineer ensures the backend features meet the required quality standards. This includes writing and executing test cases for backend logic and API responses, performing integration tests to verify inter-component communication, and using tools such as Postman or automated testing frameworks like Jest or Mocha. They identify bugs, validate fixes, and ensure a consistent and bug-free user experience throughout the development cycle.

# Technology Stack

Django

 - Purpose: A high-level Python web framework used to build the backend of the application. It enables rapid development of secure and maintainable RESTful APIs and integrates seamlessly with databases and authentication systems.

PostgreSQL

 - Purpose: A relational database management system used to store structured data such as users, properties, bookings, and transactions. It works well with Django through Django’s ORM (Object-Relational Mapping).

GraphQL

 - Purpose: An alternative to REST for API communication. It allows clients to request exactly the data they need, which can improve performance and flexibility. It is used to handle complex queries and optimize frontend-backend communication.


# Database Design

The database for the Airbnb Clone Project is structured to manage users, properties, bookings, reviews, and payments efficiently. The Users table stores details such as the user’s name, email, password, and role (host or guest). Each user can list multiple properties and make multiple bookings. The Properties table contains information about each listing, including the title, description, location, and a reference to the host (user). Each property can have multiple bookings and receive reviews from guests. The Bookings table captures data about reservations, such as check-in and check-out dates, and links to both the guest (user) and the property. The Reviews table allows users to leave ratings and comments for properties they have booked, linking each review to both a user and a property. Lastly, the Payments table records payment transactions for bookings, including the amount, payment date, and status, with each payment associated with a specific booking. These entities are relationally connected to reflect real-world interactions between users and the booking platform.

