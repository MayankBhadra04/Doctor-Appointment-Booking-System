# Doctor Appointment Booking System

A full-stack web application that connects patients with doctors. Patients can browse doctors by specialty, book and manage appointments, and pay online. Doctors and admins get dedicated dashboards for managing appointments, availability, and profiles.

## Features

- Patient registration/login with JWT authentication
- Browse and filter doctors by specialty
- Book, view, and cancel appointments with slot-based availability
- Online payments via Razorpay
- Profile management with image uploads (Cloudinary)
- Doctor dashboard for managing appointments and availability
- Admin dashboard for managing doctors and all appointments

## Tech Stack

**Backend**
- Node.js, Express
- MongoDB with Mongoose
- JWT authentication, Bcrypt password hashing
- Multer + Cloudinary for image uploads
- Razorpay for payments

**Frontend** (patient-facing app)
- React 18, Vite
- React Router v7
- Tailwind CSS
- Axios, React-Toastify

**Admin Panel**
- React 18, Vite
- React Router v7
- Tailwind CSS
- Axios, React-Toastify

## Project Structure

```
.
├── backend/    # Express API, MongoDB models, auth, payments
├── frontend/   # Patient-facing React app
└── admin/      # Admin & doctor dashboard React app
```

## Getting Started

### Prerequisites

- Node.js
- MongoDB instance (local or Atlas)
- Cloudinary account (for image uploads)
- Razorpay account (for payments)

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in `backend/` with the required environment variables (MongoDB URI, JWT secret, Cloudinary credentials, Razorpay keys, admin credentials, etc.).

```bash
npm run server   # starts with nodemon
# or
npm start
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Admin Panel Setup

```bash
cd admin
npm install
npm run dev
```

## License

ISC
