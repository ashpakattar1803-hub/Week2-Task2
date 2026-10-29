# PeoplePulse Employee Management System

Responsive employee administration dashboard built with HTML, CSS, JavaScript, Node.js, Express and MongoDB/Mongoose.

## Features
- Create, read, update and delete employee records
- Search and sort records, plus dashboard statistics
- Pre-filled edit form and delete confirmation
- Server-side Mongoose validation and unique employee ID
- REST API at `/api/employees`
- Responsive layout and team imagery

## Setup
1. Install Node.js LTS and ensure MongoDB is running locally, or create a MongoDB Atlas database.
2. Open this folder in VS Code.
3. In the terminal run `npm install`.
4. Copy `.env.example` to `.env` and set `MONGODB_URI` to your database connection string.
5. Run `npm start`.
6. Open `http://localhost:3000` in your browser. Do not open `index.html` directly; the frontend uses the Express API.

## REST endpoints
- `GET /api/employees` — list records; supports `search`, `department`, `sortBy`, and `order` query parameters
- `GET /api/employees/:id` — get one record
- `POST /api/employees` — create record
- `PUT /api/employees/:id` — update record
- `DELETE /api/employees/:id` — delete record
- `GET /api/health` — server/database status

## Employee fields
`employeeCode`, `name`, `department`, `role`, `email`, `phone`, `salary`, `joinDate`, `status`, `photoUrl`.

For real HR data, add authentication, role-based authorization, HTTPS, backups, and audit logging before deployment. Keep `.env` private and never commit it to GitHub.
