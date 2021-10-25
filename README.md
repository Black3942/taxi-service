# Taxi-service app
This is a simple application of the driver's registration system. The system user is the driver. The driver can sign up and if he already signed up - sign in. The driver can view all information about available cars and drivers assigned to them. Basic CRUD operations are available.

# Functionality
- Create a new driver (user) with the "Register" button (the user is the driver).
- Login the driver. When invalid login or password we get an "Error" message on our web page.
- Show all drivers and drivers info. Here we can delete the driver from DB. When deleting driver - the driver is unassigning from all cars.
- Show all cars and cars info. Here we can delete the car from DB (using soft delete). When deleting the car - all drivers are unssigning from this car.
- Show all manufacturers and manufacturers info. Here we can delete the manufacturer from DB.
- Add a new driver (same form like in "Register" button).
- Add a new car. Also, here we see a list of all cars for convenience.
- Add new manufacturer. Also, here we see a list of all manufacturers for convenience.
- Assign drivers to cars. Also, here we see a list of all cars and drivers for convenience.
- Show all assigned cars for the signed-in driver.
- Also, we have "Home" and "Logout" buttons.

# Technologies Used:
- Java 11
- Maven Checkstyle Plugin
- Javax Servlet API
- JSTL
- JSP
- JDBC
- Apache Tomcat
- MySQL RDBMS
- DI(custom injector)
- Log4j2

# Running the Project:

1. Fork and clone this project
2. Install MySQL
3. Install Tomcat 9.0.54 version
4. In src/main/resources directory you can find init_db.sql file. Use it to initialize you database
5. Go to the ConnectionUtil class located in src/main/java/taxi/util and add your url to DB, login, password and JDBC driver there.
   (You should add a Timezone to it too)
6. Configure your Tomcat. (Your application context needs to be as "/")
7. Run this project using Tomcat's local server