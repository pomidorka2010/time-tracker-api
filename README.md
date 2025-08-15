# Time Tracker API

## Overview
Time Tracker API is a simple RESTful application that helps users record and manage the time spent on various tasks. The application provides endpoints for creating, retrieving, updating, and deleting time entries associated with user-defined tasks.

## Features
- User authentication (JWT)
- Create, read, update, and delete task time entries
- Aggregate total time spent on tasks
- Filter time entries by date and task

## Technologies Used
- Node.js
- Express
- MongoDB
- Mongoose
- JWT for authentication

## Getting Started
### Prerequisites
- Node.js and npm installed
- MongoDB database set up

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/time-tracker-api.git
   cd time-tracker-api
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file for environment variables:
   ```
   # Add your MongoDB URI and JWT secret
   MONGODB_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   ```
4. Start the server:
   ```bash
   npm start
   ```

## API Endpoints
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login an existing user
- `GET /api/time-entries` - Get all time entries for the authenticated user
- `POST /api/time-entries` - Create a new time entry
- `PUT /api/time-entries/:id` - Update an existing time entry
- `DELETE /api/time-entries/:id` - Delete a time entry

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.