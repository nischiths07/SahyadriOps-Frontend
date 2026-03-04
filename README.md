# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


# HostelOps 🏢
### Production-Ready Hostel Complaint & Maintenance Management System

HostelOps is a centralized digital platform for managing maintenance complaints in college hostels. It uses the MERN stack and is fully containerized for easy deployment.

## 🚀 Deployment (Production Mode)

1. **Install Docker Desktop** (if not already installed).
2. **Clone the repository** (or navigate to the project directory).
3. **Run the following command** in the root directory:
   ```bash
   docker-compose up --build
   ```
4. **Access the Application**:
   - Frontend/Gateway: [http://localhost](http://localhost)
   - Backend API: [http://localhost/api/health](http://localhost/api/health)

## 🛠 Tech Stack
- **Frontend**: React, Tailwind CSS, Vite, Framer Motion, Lucide Icons
- **Backend**: Node.js, Express, MongoDB, Mongoose, JWT
- **DevOps**: Docker, Docker Compose, Nginx (Reverse Proxy)

## 📁 Project Structure
- `backend/`: Express server and MongoDB models.
- `frontend/`: React SPA with integrated Nginx production config.
- `docker-compose.yml`: Global orchestration for all services.

## 🔑 Key Features
- **Student Dashboard**: Submit complaints with priority levels and track status.
- **Admin Command Center**: Review all tickets, filter by category/status, and update statuses with remarks.
- **Security**: JWT-based authentication and role-based access control.
- **Design**: Premium glassmorphism UI with smooth animations.

## 🧪 Development Mode
To run without Docker:
1. **Backend**: `cd backend && npm install && npm start`
2. **Frontend**: `cd frontend && npm install && npm run dev`
*(Make sure MongoDB is running locally on port 27017)*
