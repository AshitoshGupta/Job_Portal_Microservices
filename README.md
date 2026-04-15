# Job Portal Microservices 🚀

A cloud-native **Job Portal Application** built using **Microservices Architecture**, designed to handle authentication, job postings, applications, resume parsing, and notifications at scale.

The project is containerized using **Docker**, images are stored in **AWS ECR**, and services are deployed using **AWS ECS Fargate** for serverless container orchestration.

---

## Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JWT
- **Containerization:** Docker
- **Cloud:** AWS ECS Fargate, ECR
- **API Communication:** REST APIs
- **Version Control:** Git, GitHub

---

## Architecture

The application follows a **microservices-based architecture** with independent services:

- **Auth Service** → Signup, Login, JWT Authentication
- **Job Service** → Create, Update, Delete, Search Jobs
- **Application Service** → Apply for jobs, Track application status
- **Resume Parser Service** → Parse uploaded resumes and extract skills
- **Notification Service** → Email/SMS notifications

Each service runs independently in its own Docker container.

---

## Project Structure

```bash
job-portal-microservices/
│
├── auth-service/
├── job-service/
├── application-service/
├── resume-parser-service/
├── notification-service/
├── docker-compose.yml
└── README.md
