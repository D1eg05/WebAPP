# WebAPP

Flight Reservation Website
Description
The Flight Reservation Website is a web application designed to allow users to book flights, manage reservations, and execute SQL queries directly on a MySQL database. The application supports registration, login, flight reservations, and querying the database for various use cases. It features a responsive design with interactive components and dynamic data handling.

Features
User Registration and Login:
Users can register with their personal details and create a secure account.
Existing users can log in to access their reservations and manage flights.
Flight Booking:
Users can book flights with options for one-way or roundtrip travel.
Fields include origin, destination, travel date, return date, number of passengers, and class.
Custom SQL Query Execution:
Execute custom SELECT SQL queries via a dedicated page.
View live query results in a dynamic table format.
Designed for admin or data exploration purposes.
Dynamic Background Effects:
Smoothly transitioning background images for a visually appealing interface.
Interactive Notifications:
Toast notifications provide feedback for successful and failed operations (e.g., login, reservation creation, query execution).
Responsive Design:
The website is fully responsive and adapts to various screen sizes and devices.



Pages
1. Home Page (index.html)
Overview of the application.
Navigation bar with links to Register, Login, and Reserve pages.
2. Register Page (register.html)
Users can create a new account by entering required details like name, email, and password.
3. Login Page (login.html)
Secure login form for existing users.
On successful login, users are redirected to their dashboard or reservation page.
4. Reservation Page (reserve.html)
Users can book flights by filling out the flight reservation form.
Options for one-way and roundtrip bookings are provided.
5. Query Page (query.html)
Admins can input and execute SELECT queries.
Query results are displayed dynamically in a table format.

Technologies Used
Frontend:
HTML5, CSS3, JavaScript
Toast notifications for user feedback
Dynamic and responsive design
Backend:
Node.js with Express.js
Sequelize ORM for database operations
Database:
MySQL
Query execution and results retrieval
Other Libraries:
bcrypt for password hashing.
mysql2 and Sequelize for database interactions.

Setup Instructions
Prerequisites
Node.js and npm installed on your machine.
MySQL database set up with a test database.
Steps
Clone the repository:
bash
Copy code
git clone <repository-url> 
cd FlightReservation


Install dependencies:
bash
Copy code
npm install


Configure the database:
Ensure MySQL is running.
Edit the database configuration in DAO.js or model.js to match your MySQL credentials.
Run the server:
bash
Copy code
node index.js


The application will start at http://localhost:3000.
Access the website:
Open your browser and navigate to http://localhost:3000.





Usage
Register a New User:
Go to the Register page and create a new account. 
Login:
Login with your credentials to access flight booking.
Book Flights:
Navigate to the Reserve page to book flights.
Execute Queries:
Go to the Query page and input SQL SELECT queries to fetch data directly from the database.
Folder Structure
java
Copy code
FlightReservation/
├── public/
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── reserve.html
│   ├── query.html
│   ├── style.css
│   ├── main.js
├── model.js
├── DAO.js
├── database.js
├── index.js
├── package.json
├── package-lock.json






Troubleshooting
Database Connection Issues:
Ensure MySQL is running.
Verify database credentials in DAO.js.
Module Not Found Errors:
Ensure all dependencies are installed using npm install.
Query Execution Issues:
Ensure the query starts with SELECT.
Check MySQL permissions for the configured user.

