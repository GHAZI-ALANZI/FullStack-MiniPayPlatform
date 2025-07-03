# MiniPayPlatform 💳

A full-stack microservice-based payment platform with ASP.NET Core backend (DDD architecture) and React frontend. This project simulates a minimal payment processing service with mock API interactions.

---
<img width="892" alt="Image" src="https://github.com/user-attachments/assets/aee6cac5-2e1d-47fe-9b8c-dc5187ae5b04" />



<img width="867" alt="Image" src="https://github.com/user-attachments/assets/cf38e29c-fcc0-4e36-a915-a30f73f92083" />



<img width="336" alt="Image" src="https://github.com/user-attachments/assets/c245b0ca-749e-47de-bc12-9b2fca5fba6e" />


## 📁 Project Structure

MiniPayPlatform/
│
- ├── backend/ # ASP.NET Core 8 Web API (DDD)
- │ ├── MiniPayPlatform.API/ # API Layer (Controllers)
- │ ├── MiniPayPlatform.Application/ # Application Layer (DTOs, Interfaces)
- │ ├── MiniPayPlatform.Domain/ # Domain Layer (Entities, Enums)
- │ ├── MiniPayPlatform.Infrastructure/ # Infrastructure Layer (Persistence, Configs)
- │ └── MiniPayPlatform.Tests/ # Unit Tests (xUnit, Moq)
- │
- ├── frontend/ # React SPA (Vite, Axios, Bootsrap)
- │ ├── src/
- │ │ ├── components/
- │ │ ├── services/
- │ │ ├── types/
- │ │ └── App.jsx
- │ └── public/
- │
- └── README.md



## 🚀 Tech Stack

### 🔧 Backend
- ASP.NET Core Web API
- Domain-Driven Design (DDD)
- Entity Framework Core 
- AutoMapper
- xUnit + Moq (Unit Testing)
- RESTful APIs

### 💻 Frontend
- React 19
- Vite
- Axios
- React Router
- Bootstrap

---

## 🧠 Features

### Backend (ASP.NET Core)
- CRUD operations for Payment Providers
- RESTful endpoints
- DDD architecture with layered separation
- AutoMapper support
- Standardized `ApiResponse<T>` for all results
- Mock API integration for payment simulation

### Frontend (React)
- Display and manage payment providers
- Consume backend APIs using Axios
- Simple and clean UI

---

## 📦 Getting Started

### Prerequisites
- [.NET 8 SDK](https://dotnet.microsoft.com/download)
- [Node.js](https://nodejs.org/)
- [Git](https://git-scm.com/)

---

## 🛠 Setup Instructions

### 1️⃣ Clone the main repo

git clone https://github.com/your-username/FullStack-MiniPayPlatform.git
cd FullStack-MiniPayPlatform
2️⃣ Add submodules

# Add backend as a submodule
git submodule add https://github.com/GHAZI-ALANZI/MiniPayPlatform.git

# Add frontend as a submodule
git submodule add https://github.com/GHAZI-ALANZI/ClientAppMiniPay.git
💡 Note: You may need to commit .gitmodules file and run git submodule update --init --recursive if cloning later.

⚙️ Backend (ASP.NET Core)

cd MiniPayPlatform
dotnet build
dotnet run
Runs on: https://localhost:7128

Test it via Swagger or Postman:

GET     /api/v1/paymentprovider
GET     /api/v1/paymentprovider/{id}
POST    /api/v1/paymentprovider
PUT     /api/v1/paymentprovider/{id}
DELETE  /api/v1/paymentprovider/{id}
POST    /api/v1/PaymentSimulation/simulate-payment

🎨 Frontend (React)

cd ClientAppMiniPa
npm install
npm run dev
Runs on: http://localhost:5173

Ensure CORS is configured properly in the backend for frontend to connect.

🧪 Testing
Run Backend Unit Tests

cd MiniPayPlatform/MiniPayPlatform.Tests
dotnet test

## 🛣 MiniPayPlatform Roadmap (Backend + Frontend)


## 🚧 Phase 1 – Core Improvements
Backend

Connect real DB (SQL Server/Postgres)

Validation, error handling, logging

Pagination, filtering

Frontend

Form validation, loading states

Pagination UI, search filter

Toast notifications

## 🔐 Phase 2 – Auth & Security
Backend

JWT authentication

Role-based access

HTTPS & CORS config

Frontend

Login/logout flow

Auth guard for protected routes


## 🚀 Phase 3 – Deployment
Backend

Dockerize API

GitHub Actions for CI/CD

Health checks, monitoring

Frontend

Docker + static build

Deploy to Vercel/Netlify

GitHub Actions for CI/CD



## 🙋‍♂️ Author
- Ghazi Alanzi
