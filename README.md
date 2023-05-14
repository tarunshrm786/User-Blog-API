# User-Blog-API
User, Blog Management API, which uses nodejs, expressjs, mongodb.

This project provides a set of APIs for managing users and blogs, with additional functionality for admin users. It is built using Node.js, Express.js, and MongoDB.

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/admin-apis.git`
2. Install the dependencies: `npm install`
3. Set up the MongoDB connection by updating the `config/database.js` file with your MongoDB connection details.
4. Start the server: `npm start`

The server will start running on `http://localhost:7700`.

## API Endpoints

### User Management (for Admins)

- `GET /api/admin/users`: Retrieve a list of all users.
- `GET /api/admin/users/:id`: Retrieve user information by ID.
- `PUT /api/admin/users/:id`: Update user information by ID. Required parameters: name, age, address.
- `DELETE /api/admin/users/:id`: Delete a user by ID.

### Authentication

- `POST /api/auth/login`: Log in as an admin using hardcoded email and password.

### Blog Management

- `GET /api/blogs`: Retrieve a list of all blogs.
- `POST /api/blogs`: Create a new blog. Required parameters: title, content, images.
- `GET /api/blogs/:id`: Retrieve blog information by ID.
- `PUT /api/blogs/:id`: Update blog information by ID. Required parameters: title, content, images.
- `DELETE /api/blogs/:id`: Delete a blog by ID.


