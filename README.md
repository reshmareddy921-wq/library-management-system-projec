# Library Management System projec

Academic beginner full-stack project based on the supplied documentation.

## Features
- Dashboard counts (books, members, active issues, returned books)
- Book CRUD
- Member CRUD
- Issue books (only when available)
- Return books
- Transaction history
- MongoDB persistence

## Requirements
- Node.js 18+
- MongoDB local installation or MongoDB Atlas connection string

## Setup

### 1. Backend
```bash
cd server
npm install
cp .env.example .env
# Edit MONGO_URI if needed
npm run dev
```
Backend runs at `http://localhost:5000`.

### 2. Frontend
Open another terminal:
```bash
cd client
npm install
npm run dev
```
Frontend runs at `http://localhost:5173`.

## Default API
- `GET /api/books`, `POST /api/books`, `PUT /api/books/:id`, `DELETE /api/books/:id`
- `GET /api/members`, `POST /api/members`, `PUT /api/members/:id`, `DELETE /api/members/:id`
- `GET /api/transactions`
- `POST /api/transactions/issue`
- `PUT /api/transactions/:id/return`
- `GET /api/dashboard`

This is an academic starter, not a production-ready system. Add authentication, authorization, validation, and deployment configuration before production use.
