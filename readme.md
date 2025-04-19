# Kanban Board Application

A full-stack Kanban board application built with Express, TypeScript, and MySQL.

🚀 [Live Demo](https://kanban-board-app.onrender.com)

## Demo Credentials
To try the application, use these credentials:
- **Username:** JollyGuru
- **Password:** password

## Description

This project is a task management system that allows users to organize their work using a Kanban board interface. Users can create tickets, track their progress, and manage their workflow efficiently.

## Features

- User authentication and authorization
- Ticket creation and management
- Drag-and-drop interface for ticket status updates
- Secure API endpoints
- Database persistence

## Technology Stack

- **Backend:**
  - Node.js with Express
  - TypeScript
  - MySQL database
  - Sequelize ORM
  - JSON Web Tokens for authentication

- **Frontend:**
  - React (presumed based on project structure)
  - TypeScript
  - Modern CSS

## Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
```

2. Install dependencies:
```bash
cd kanbanBoard
npm install
```

3. Set up the database:
```bash
mysql -u root -p < server/db/schema.sql
```

4. Create a `.env` file in the root directory:
```env
DB_NAME='kanban_db'
DB_USER='your_username'
DB_PASSWORD='your_password'
JWT_SECRET='your_secret_key'
```

5. Seed the database:
```bash
npm run seed
```

## Usage

1. Start the development server:
```bash
npm run dev
```

2. Access the application at `http://localhost:3000`

## API Endpoints

- **Authentication**
  - POST `/api/auth/login` - User login
  - POST `/api/auth/register` - User registration

- **Users**
  - GET `/api/users` - Get all users
  - GET `/api/users/:id` - Get user by ID

- **Tickets**
  - GET `/api/tickets` - Get all tickets
  - POST `/api/tickets` - Create new ticket
  - PUT `/api/tickets/:id` - Update ticket
  - DELETE `/api/tickets/:id` - Delete ticket

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Default Users

The application comes with three seeded users:
- JollyGuru
- SunnyScribe
- RadiantComet

All seeded users have the password: `password`