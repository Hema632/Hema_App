# RemindMe - MERN Stack Reminder Application

A comprehensive reminder application built with the MERN stack (MongoDB, Express, React, Node.js) that helps users manage their daily tasks and reminders.

## Features

- User authentication (signup, login, logout)
- Create, read, update, and delete reminders
- Set due dates and times with optional recurrence
- Priority levels with visual indicators
- Category/tag system for organizing reminders
- Search and filter capabilities
- Responsive design for all devices

## Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS, Lucide Icons
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT
- **Form Handling**: React Hook Form
- **Date Management**: date-fns

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas)

## Setup & Installation

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Configure environment variables:
   Create a `.env` file in the root directory with the following variables:
   ```
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   NODE_ENV=development
   ```

4. Run the development server:
   ```
   npm run dev:all
   ```
   This will start both the frontend and backend servers concurrently.

## Project Structure

```
reminder-app/
├── public/              # Static files
├── server/              # Backend code
│   ├── middleware/      # Express middleware
│   ├── models/          # Mongoose models
│   ├── routes/          # API routes
│   └── server.js        # Entry point
├── src/                 # Frontend code
│   ├── components/      # React components
│   ├── context/         # React context
│   ├── pages/           # Page components
│   ├── App.tsx          # Main app component
│   └── main.tsx         # Entry point
├── .env                 # Environment variables
├── package.json         # Dependencies
└── README.md            # Project documentation
```

## API Endpoints

### Authentication
- `POST /api/users` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth` - Get logged in user

### Reminders
- `GET /api/reminders` - Get all reminders for a user
- `POST /api/reminders` - Create a new reminder
- `PUT /api/reminders/:id` - Update a reminder
- `DELETE /api/reminders/:id` - Delete a reminder

## Future Enhancements

- Email notifications
- Calendar view integration
- Sharing reminders with other users
- Mobile application using React Native
- Dark/light theme toggle
- Advanced recurring reminder patterns