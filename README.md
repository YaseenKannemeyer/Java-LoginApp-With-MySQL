## Java Login App With MySQL
A simple Java web application with a login page that verifies users against a MySQL database using a servlet. Currently supports read-only login verification and will be updated to include write functionality soon.

### 📋 Features
-Web-based login form built with HTML, CSS, and JavaScript

-Backend Java Servlet (LoginServlet) handles login POST requests

-Validates user credentials against a MySQL database

-Displays success or error messages dynamically on the page

-Uses JDBC with MySQL Connector/J driver

-Runs on Apache Tomcat server

  ⚠️ Currently, the app only supports reading/validating credentials. Write/update user functionality will be implemented in future updates.

### 🛠️ Technologies Used
-Java 24 (Servlet API with Jakarta EE)

-MySQL database

-MySQL Connector/J JDBC driver

-Apache Tomcat

-HTML, CSS, JavaScript (fetch API)

### 🗂 Project Structure
```graphql
Copy
Edit
LoginApp/
├── src/
│   └── LoginServlet.java  # Servlet handling login POST requests
├── web/
│   └── index.html         # Login page with form and JS
├── .gitignore             # Ignoring build and IDE files
└── README.md
```


###💻 Installation & Usage


1. Clone the repo:

```bash

git clone https://github.com/YaseenKannemeyer/Java-LoginApp-With-MySQL.git
```
2. Import the project into your preferred IDE (e.g., NetBeans, IntelliJ IDEA).

3. Set up MySQL database:

--Create database loginapp

--Create table users with columns username and password

--Add some test users for login

4. Update your database credentials in LoginServlet.java or switch to config/environment variables (recommended).

5. Build and deploy the app on Apache Tomcat server.

6. Open the login page (index.html) in a browser and test login.

### 🚀 How It Works
-User enters username and password on the login page.

-JavaScript captures form submission and sends a POST request to /LoginServlet.

-Servlet connects to MySQL, checks if credentials exist.

-Responds with success or failure text.

-JavaScript displays an appropriate message on the page.

### 🔐 Security Notice
-Currently, credentials are hardcoded in the servlet for demonstration only.

-For production, never commit secrets to code. Use environment variables or config files excluded by .gitignore.

-Change your DB password if exposed.

### 📞 Contact
-For questions or collaboration:

-Email: yaseenkannemeyer@gmail.com

-GitHub: YaseenKannemeyer

### 📄 License
-This project is in the public domain. Feel free to use and modify it freely.

© 2025 Mogamat Yaseen Kannemeyer

