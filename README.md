Donation Manager – Docker Setup
This project contains the Dockerized version of the Donation Manager application, which includes:
- A Spring Boot backend
- An Angular frontend
- A MySQL database

Prerequisites:
- Docker
- Docker Compose

Backend: https://github.com/kedith/backend
Frontend: https://github.com/kedith/frontend

How to Run:
- Make sure you are in the root of the donation-manager project, then run:
docker-compose up --build

The services will start as follows:
- Frontend: http://localhost:4200
- Backend (API): http://localhost:8080

MySQL Database: accessible on port 3307

📁 Project Structure
Copy
Edit
donation-manager/
│
├── backend/
│   ├── Dockerfile
│   └── ... (Spring Boot application)
│
├── frontend/
│   ├── Dockerfile
│   └── ... (Angular application)
│
├── docker-compose.yml
└── README.md

🐳 Docker Images
- donation-manager-backend: Builds the backend JAR and runs it in a lightweight Java container.
- donation-manager-frontend: Builds the Angular app and serves it via Nginx.
- mysql-db: Uses the official MySQL image with port mapping and environment setup.
