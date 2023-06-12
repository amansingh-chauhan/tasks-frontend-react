Task Manager App
This is a Task Manager application built with React.js on the frontend and Node.js on the backend. It allows users to register, log in, create tasks, mark tasks as completed, and delete tasks. The application uses React Router for navigation and Axios for making HTTP requests to the backend API.

Features
User registration: Users can create an account by providing their name, email, and password.
User login: Registered users can log in using their email and password.
User profile: Users can view their profile information once logged in.
Task creation: Logged-in users can create tasks by providing a title and description.
Task list: Users can view their own tasks on the home page, including the title, description, and completion status.
Task completion: Users can mark a task as completed by checking a checkbox associated with the task.
Task deletion: Users can delete a task from their task list.
Logout: Users can log out of their account.
Technologies Used
React.js
Node.js
Express.js
MongoDB
React Router
Axios
bcrypt
Getting Started
To run this application locally, follow the steps below:

Clone the repository:

bash
Copy code
git clone <repository-url>
Install the dependencies for both the frontend and backend:

bash
Copy code
# Navigate to the frontend directory
cd frontend
npm install

# Navigate to the backend directory
cd ../backend
npm install
Set up the environment variables:

Create a .env file in the backend directory.

Add the following environment variables to the .env file:

makefile
Copy code
MONGO_URI=<your-mongodb-uri>
SECRET_KEY=<your-secret-key>
Replace <your-mongodb-uri> with your MongoDB connection string and <your-secret-key> with a secret key for JWT token generation.

Start the development servers:

bash
Copy code
# Start the frontend development server
cd frontend
npm start

# Start the backend development server
cd ../backend
npm start
Open your browser and visit http://localhost:3000 to access the application.

API Endpoints
The backend API provides the following endpoints:

POST /users/register: Register a new user.
POST /users/login: Log in an existing user.
GET /users/me: Get the authenticated user's profile data.
GET /users/logout: Log out the authenticated user.
POST /task/new: Create a new task.
GET /task/my: Get the tasks of the authenticated user.
PUT /task/:id: Update the completion status of a task.
DELETE /task/:id: Delete a task.
Contributing
Contributions to this project are welcome. You can contribute by submitting bug reports, feature requests, or pull requests.

To submit a bug report or feature request, please use the GitHub issue tracker.
To submit a pull request, please follow these steps:
Fork the repository.
Create a new branch for your feature or bug fix.
Make the necessary changes in your branch.
Commit and push your changes to your forked repository.
Submit a pull request to the main repository.
