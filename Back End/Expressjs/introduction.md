## Lesson 1: Introduction to Express.

### Overview of Express and its role in web development:

**Express.js:**
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. It simplifies the process of building web applications by providing a set of tools for creating routes, handling requests and responses, and managing middleware.

**Role in Web Development:**
Express is commonly used for building server-side applications and APIs. Its lightweight and unopinionated nature make it a popular choice for developers who want flexibility and control over their application's structure. Express is particularly well-suited for building RESTful APIs and single-page applications.

### Installation and setup of Node.js and Express:

**1. Install Node.js:**
   - Visit the [official Node.js website](https://nodejs.org/).
   - Download and install the latest version of Node.js for your operating system.

**2. Verify Node.js Installation:**
   - Open a terminal or command prompt.
   - Run the following commands to check if Node.js and npm (Node Package Manager) are installed:
     ```bash
     node -v
     npm -v
     ```

**3. Install Express:**
   - In the terminal, navigate to your project folder.
   - Run the following command to initialize a new Node.js project (creates a `package.json` file):
     ```bash
     npm init -y
     ```
   - Install Express using npm:
     ```bash
     npm install express
     ```

### Creating a basic Express application:

**1. Set Up Your Project:**
   - Create a new file (e.g., `app.js` or `index.js`) for your Express application.

**2. Import Express:**
   - In your JavaScript file, import Express by adding the following lines:
     ```javascript
     const express = require('express');
     const app = express();
     ```

**3. Create a Basic Route:**
   - Define a simple route to handle HTTP GET requests:
     ```javascript
     app.get('/', (req, res) => {
       res.send('Hello, Express!');
     });
     ```

**4. Start the Server:**
   - Add code to start the Express server and listen on a specific port (e.g., 3000):
     ```javascript
     const PORT = 3000;
     app.listen(PORT, () => {
       console.log(`Server is running on http://localhost:${PORT}`);
     });
     ```

**5. Run Your Application:**
   - In the terminal, run your application using the following command:
     ```bash
     node app.js
     ```
     Visit `http://localhost:3000` in your browser, and you should see "Hello, Express!".

Congratulations! You've created a basic Express application. This sets the foundation for building more complex web applications using Express. 
Feel free to experiment with different routes and responses to deepen your understanding.
