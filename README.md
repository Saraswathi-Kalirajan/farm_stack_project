# farm_stack_project 

A modern full-stack To-Do List app designed to help you organize your tasks effortlessly. This project combines a powerful *FastAPI* backend with a sleek *React* frontend, backed by *MongoDB Atlas* for reliable data persistence.

---

## 🚀 Project Highlights

- Complete CRUD operations for managing to-do lists and individual tasks  
- Built with asynchronous Python and FastAPI for high performance  
- Responsive React UI for an intuitive user experience  
- Cloud-ready MongoDB Atlas integration  
- Containerized using Docker and Docker Compose for easy deployment  
- NGINX as a reverse proxy to route frontend and backend requests  

---

## 🛠 Tools Used

- *FastAPI* — Backend API framework  
- *React* — Frontend UI library  
- *MongoDB Atlas* — Cloud-hosted NoSQL database  
- *Motor* — Async MongoDB driver for Python  
- *Axios* — HTTP client for frontend API calls  
- *Docker & Docker Compose* — Containerization and orchestration  
- *NGINX* — Reverse proxy configuration  
- *Uvicorn* — ASGI server to run FastAPI  

---

## 🌐 Tech Stack

- Python  
- JavaScript (React)  
- MongoDB (NoSQL)  
- Docker  

---

## 💻 Local Setup Instructions

### Prerequisites

- Docker and Docker Compose installed  
- MongoDB Atlas cluster with connection URI  

### Steps

1. *Clone the repository:*

   ```bash
   git clone https://github.com/Saraswathi-Kalirajan/farm_stack_project.git
   cd farm_stack_project
   2. Create a .env file in the root directory and add your MongoDB connection string:

MONGODB_URI="mongodb+srv://saraswathik729:saras1206@cluster0.h5mj6lr.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0"


3. Build and start the containers:

docker-compose up --build


4. Access the application:

Frontend UI: http://localhost:3000

API Docs: http://localhost:3001/docs



5. To stop and clean up the environment:

docker-compose down --volumes --remove-orphans




---

## 🎥 Demo Video

[▶ Watch Demo Video](https://drive.google.com/file/d/1VfS1wss6cCpvAadN7TOJMkVHM9NN13_0/view?usp=drivesdk)