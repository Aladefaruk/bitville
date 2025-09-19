# Bitville - User Management Application

A full-stack web application for managing users and their posts, built with TypeScript, React, and Node.js.

## Overview

Bitville is a modern user management system that allows you to browse users, view their posts, and manage content through an intuitive interface. The application features a clean, responsive design and robust error handling.

## Tech Stack

### Backend
- **Node.js** with **TypeScript**
- **SQLite** database for data persistence
- **Express.js** for RESTful API endpoints
- Comprehensive error handling and validation

### Frontend
- **React** with **TypeScript**
- **React Query** for efficient state management
- **Tailwind CSS** for responsive styling
- **React Testing Library** for unit testing

## Features

### User Management
- Browse users with pagination (4 users per page)
- View user details including full name, email, and formatted address
- Responsive table design with overflow handling

### Post Management
- View all posts for a specific user
- Create new posts with title and body
- Delete posts with confirmation
- Real-time UI updates without page refresh

### Technical Features
- Efficient data fetching and caching with React Query
- Loading and error states for all operations
- Responsive design for various screen sizes
- Clean component architecture with separation of concerns
- Comprehensive unit testing

## API Endpoints

### Users
- `GET /users` - Get paginated list of users
- `GET /users/count` - Get total user count

### Posts
- `GET /posts?userId={id}` - Get posts for a specific user
- `POST /posts` - Create a new post
- `DELETE /posts/:id` - Delete a post by ID

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- pnpm (or npm/yarn)

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
pnpm install
```

3. Start the backend server:
```bash
pnpm start
```

The backend server will run on `http://localhost:3001`

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
pnpm install
```

3. Start the frontend development server:
```bash
pnpm start
```

The frontend will run on `http://localhost:3000`

### Running Tests

To run the frontend unit tests:
```bash
cd frontend
pnpm test
```

### Database

The SQLite database (`data.db`) is already included in the backend directory with sample data. No additional setup is required.

## Project Structure

```
bitville/
├── backend/          # Node.js TypeScript server
│   ├── src/         # Source code
│   └── data.db      # SQLite database
└── frontend/        # React TypeScript application
    ├── src/         # Source code
    └── public/      # Static assets
```

## Contributing

This project follows modern development practices:
- TypeScript for type safety
- Component-based architecture
- Efficient state management with React Query
- Comprehensive error handling
- Unit testing for critical functionality
- Responsive design principles

