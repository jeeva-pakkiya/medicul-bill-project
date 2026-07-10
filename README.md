# Easy To Bill — Medical Billing & Inventory Management System

A production-ready full-stack medical billing system built with React.js + FastAPI + MySQL.

## Tech Stack
- **Frontend**: React.js (Vite) + Tailwind CSS v4
- **Backend**: Python FastAPI + SQLAlchemy 2.0 (async) + MySQL
- **Auth**: JWT (PyJWT + Argon2id password hashing)
- **Charts**: Chart.js via react-chartjs-2
- **Print/PDF**: Browser Print API

## Default Login
```
Username: admin
Password: admin123
```

## Project Structure
```
medical bill/
├── backend/          # FastAPI Python backend
└── frontend/         # React.js frontend
```

## Setup & Run

### 1. Backend Setup
```powershell
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```
The backend will:
- Auto-create the `easy_to_bill` MySQL database
- Auto-create all tables
- Auto-create the default admin user (admin/admin123)

**Requirements**: MySQL running on localhost:3306 with user `root` / password `root`

### 2. Frontend Setup
```powershell
cd frontend
npm install
npm run dev
```
Open http://localhost:5173

## Features
- ✅ JWT Login Authentication
- ✅ Billing with searchable medicine dropdown
- ✅ Auto-increment bill numbers (starts at 1001)
- ✅ Stock deduction on billing
- ✅ Customer tracking with expected next visit
- ✅ Bill History with search and date filters
- ✅ Low Stock Alerts (Wanted page)
- ✅ Usage Analytics with Chart.js
- ✅ Sale Dashboard with revenue charts
- ✅ Invoice Print (Browser Print API)
- ✅ Global Search (medicines, customers, bills)
- ✅ Keyboard shortcuts (Ctrl+S save, Ctrl+P print)
- ✅ Responsive design (mobile-friendly)

## Database Configuration
Edit `backend/.env` to change MySQL connection:
```
DATABASE_URL=mysql+aiomysql://root:root@localhost:3306/easy_to_bill
```
"# medicul-bill-project" 
