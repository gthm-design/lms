# Library Management System (MERN Stack)

A straightforward Library Management System built with MongoDB, Express, React, and Node.js.

## Features

- **Dashboard**: Displays Total Books, Total Copies, Issued Copies, Overdue Books, Total Fine Collected, and a Recently Issued Books table.
- **Books Management**: Search by book code, title, or author; filter by category and availability; paginate results; add, view, edit, issue, and delete books.
- **Book Issuing & Returning**: Issue available copies to borrowers with due dates, automatically track overdue loans, and record returns with fine calculation.
- **Loan History**: Search and filter all loans by status (`Issued`, `Overdue`, `Returned`).

## Prerequisites

- Node.js (v18+)
- MongoDB running locally on `mongodb://127.0.0.1:27017/library_management` (or update `server/.env`)

## Setup & Running

### 1. Start the Backend Server

```bash
cd server
npm install
npm run dev
```

The API server runs on `http://localhost:5000`.

### 2. Start the Frontend Client

```bash
cd client
npm install
npm run dev
```

The React app runs on `http://localhost:5173` and proxies `/api` requests to `http://localhost:5000`.
