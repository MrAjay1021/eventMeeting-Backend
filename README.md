# Event Scheduling Application

A complete event scheduling and meeting management system with user authentication, event creation, booking, and calendar management features.

## Setup Instructions

1. **Prerequisites**
   - Node.js (v14 or later)
   - MongoDB account (or local MongoDB installation)
# Event App Backend

Express.js based API backend for the Event Scheduling Application.

## Setup Instructions

1. **Install Dependencies**
   ```bash
   npm install
- `npm run backend` - Runs only the backend
- `npm run install-all` - Installs dependencies for all parts

2. **Environment Configuration**
   - Create a `.env` file with the following variables:
     ```
     PORT=5000
     MONGODB_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     JWT_EXPIRE=30d
     ```

3. **Start Development Server**
   ```bash
   npm run dev
   ```

   The API will run on [http://localhost:5000](http://localhost:5000)

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/user` - Get current user

### Users
- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get user by ID
- `PUT /api/users/:id` - Update user
- `DELETE /api/users/:id` - Delete user

### Events
- `POST /api/events` - Create new event
- `GET /api/events` - Get all events
- `GET /api/events/:id` - Get event by ID
- `PUT /api/events/:id` - Update event
- `DELETE /api/events/:id` - Delete event

### Meetings
- `POST /api/meetings` - Create new meeting
- `GET /api/meetings` - Get all meetings
- `GET /api/meetings/:id` - Get meeting by ID

### Bookings
- `POST /api/bookings` - Create new booking
- `GET /api/bookings` - Get all bookings
- `GET /api/bookings/:id` - Get booking by ID

## Data Models

- **User** - User profile and authentication information
- **Event** - Event type templates created by users
- **Meeting** - Scheduled meetings based on events
- **Booking** - Booking information for meetings

## Key Features

- User authentication (signup, login)
- Event creation and management
- Meeting scheduling with customizable availability
- Event booking system
- Profile management
- Calendar integration
- Real-time notifications

## Architecture
- **Backend:** Express.js and Node.js
- **Database:** MongoDB (MongoDB Atlas)
- **Authentication:** JWT (JSON Web Tokens)
  
## Technologies Used

- Express.js
- MongoDB with Mongoose
- JWT Authentication
- bcrypt for password hashing
- CORS middleware for cross-origin requests

## Demo Credentials

For testing purposes, you can use:
- **Email:** demo@example.com
- **Password:** demopassword 


