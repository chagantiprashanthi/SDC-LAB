PROGRAM 7 – Session Management in Shopping Cart Web Application

AIM
To implement session tracking in a shopping cart web application using HTTP Sessions in Java Servlets.
![Screenshot (27)](https://github.com/user-attachments/assets/bc10015e-f040-4997-a0e4-87b911c63b4b)
![Screenshot (28)](https://github.com/user-attachments/assets/2e79a1bb-3adf-4a44-a0a0-2de84104d5c8)

DESCRIPTION
This experiment demonstrates how to maintain user-specific data (such as a shopping cart) using HTTP sessions in Java Servlets. When a user adds products to the cart, the servlet tracks the session and stores cart data in memory without requiring a database write for every interaction. This implementation improves performance and user experience by keeping state between page requests.

The solution uses Java Servlets for backend processing, HTML/CSS for frontend interface, and the built-in session management API provided by the servlet framework.

PROJECT STRUCTURE
shopping-cart-session/
│
├── src/
│   └── servlets/
│       ├── ProductServlet.java         # Lists products
│       └── CartServlet.java            # Handles add-to-cart with session
│
├── WebContent/
│   ├── index.html                      # Welcome page
│   ├── catalog.html                    # Displays product list with add buttons
│   ├── cart.html                       # Displays cart contents from session
│   └── WEB-INF/
│       ├── web.xml                     # Servlet and session config
│       └── lib/
│           └── mysql-connector-j-9.3.0.jar
│
├── bin/                                # Compiled .class files
├── lib/
│   └── javax.servlet-api-4.0.1.jar
├── README.md                           # Project documentation


  
INSTALLATION & SETUP
PREREQUISTIES
•	Java JDK
•	Apache Tomcat
•	MySQL
•	VS Code with Java Extensions
•	Servlet API (javax.servlet-api-4.0.1.jar)

STEPS TO RUN THE PROJECT
1.	Add Required JARs to lib/:
o	mysql-connector-j-9.3.0.jar
o	javax.servlet-api-4.0.1.jar
2.	Compile Servlets:
javac -cp "lib/*" -d bin src/servlets/ProductServlet.java src/servlets/CartServlet.java

3.	Deploy to Tomcat:
o	Copy WebContent/ into tomcat/webapps/shopping-cart-session/
o	Copy compiled bin/ classes to WEB-INF/classes/
4.	Start Tomcat Server
5.	Visit in Browser:
6.	http://localhost:8080/shopping-cart-session/index.html

DATABASE SETUP
Database: shopping_cart
Table: products
CREATE TABLE products (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(100),
  price DECIMAL(10,2)
);

LICENSE
This project is licensed under the MIT License.
