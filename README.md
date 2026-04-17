# HNG Stage 1 – DevOps API Deployment

## 📌 Project Description

This project is part of the HNG Internship Stage 1 (DevOps Track).

It is a simple API built and deployed on a Linux server. The application runs on a local port and is exposed publicly using Nginx as a reverse proxy.

---

## 🚀 Live URL

http://blessingeo.redirectme.net

---

## 💻 How to Run Locally

### 1. Clone the repository

git clone https://github.com/Enoredia/api-deployment.git  
cd api-deployment

---

### 2. Create and activate a virtual environment

python3 -m venv venv  
source venv/bin/activate

---

### 3. Install dependencies

pip install -r requirements.txt

---

### 4. Run the application

python app.py

---

### 5. Test locally

curl http://127.0.0.1:5000/  
curl http://127.0.0.1:5000/health  
curl http://127.0.0.1:5000/me

---

## 🔗 API Endpoints

### GET /

Response:
{
  "message": "API is running"
}

---

### GET /health

Response:
{
  "message": "healthy"
}

---

### GET /me

Response:
{
  "name": "Blessing Osarumwense",
  "email": "enorediabeo@gmail.com",
  "github": "https://github.com/Enoredia"
}

---

## 🧠 Notes

- All endpoints return HTTP 200  
- All responses are in JSON format  
- The API runs on a local port and is exposed via Nginx reverse proxy  
- The service is managed to run persistently on the server  
