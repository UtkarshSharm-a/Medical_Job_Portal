AI-Assisted Development
🏥 MedExJob.com – Medical Job Portal
📖 Project Overview

MedExJob.com is a comprehensive medical job portal that connects healthcare professionals with employers. The platform enables job discovery, recruitment, and secure communication within the healthcare ecosystem.

🏗️ Project Structure
MedExJobUpdated/
├── backend/          # Spring Boot Backend API (Java)
├── frontend/         # React + TypeScript Frontend (Vite)
├── deployment/       # Deployment scripts and guides
└── README.md         # Project documentation

🚀 Quick Start (Local Development)
Option 1: Quick Start Script (Recommended)

Windows

.\start-local.ps1


Linux / Mac

chmod +x start-local.sh
./start-local.sh

Option 2: Manual Setup
1️⃣ Database Setup
CREATE DATABASE medtech_db;

2️⃣ Backend Setup
cd backend
mvn clean install
mvn spring-boot:run


✅ Backend URL:
👉 http://localhost:8081

3️⃣ Frontend Setup (Open a new terminal)
cd frontend
npm install
npm run dev


✅ Frontend URL:
👉 http://localhost:5173

📋 Detailed Setup Guides

LOCAL_SETUP.md – Complete local development guide

QUICK_START.md – Quick reference guide

SETUP_CHECKLIST.md – Setup checklist and common issues

🛠️ Tech Stack
Backend

Java 17

Spring Boot 3.2.0

Spring Security (JWT Authentication)

Spring Data JPA

MySQL 8.0

Maven

Frontend

React 18

TypeScript

Vite

Tailwind CSS

Radix UI

React Router

📁 Important Files
Backend Configuration

backend/src/main/resources/application.yml – Main configuration

backend/pom.xml – Maven dependencies

Frontend Configuration

frontend/vite.config.ts – Vite configuration

frontend/package.json – npm dependencies

🔧 Configuration
Database

Database Name: medtech_db

Port: 3306 (MySQL default)

Credentials: Update in
backend/src/main/resources/application.yml

Ports
Service	Port
Backend	8081
Frontend	5173
MySQL	3306
✅ Verification
Backend Health Check
http://localhost:8081/api/actuator/health


Expected Response

{"status":"UP"}

Frontend
http://localhost:5173


Expected Result: Homepage loads successfully.

🐛 Troubleshooting

For common issues and solutions, refer to SETUP_CHECKLIST.md.

📦 Production Build
Backend
cd backend
mvn clean package


📦 JAR output:

target/medexjob-backend-1.0.0.jar

Frontend
cd frontend
npm run build


📦 Build output:

dist/

🚀 Deployment

For deployment on Hostinger, refer to the guides inside the deployment/ folder.

📝 Development Workflow

Local Development – Follow this guide

Testing – Test all features locally

Production Build – Use build commands

Deployment – Follow deployment guides

🔐 Security Notes

Change JWT secret in production

Keep database credentials secure

Use environment variables for production configuration

📞 Support & Debugging

If you face issues:

Check backend logs:
backend/logs/medexjob.log

Check browser console (F12)

Check backend terminal for errors

📄 License

This project is licensed under the MIT License.

🎉 Happy Coding!

If you want, I can:

Make this more recruiter-friendly

Add architecture diagram section

Add API documentation section

Optimize it for GitHub stars & open-source look

Just tell me 😄
