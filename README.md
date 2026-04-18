# 📊 User Activity Analytics & Reporting System

A backend-focused system to track user activity, generate analytics, and automate reporting.  
This project simulates real-world logging and analytics pipelines used in scalable applications.

---

## 🚀 Features

- Track user activity (login, actions, events)
- Real-time event ingestion via REST APIs
- Generate analytics:
  - Daily Active Users (DAU)
  - Event frequency
  - Usage trends
- Automated report generation using scheduled jobs
- Structured storage of logs for efficient querying

---

## 🛠️ Tech Stack

- Backend: Node.js, Express.js  
- Database: MongoDB  
- Scheduling: node-cron  

---

## 📂 Project Structure
├── controllers/
├── routes/
├── models/
├── services/
├── utils/
├── config/
├── app.js
└── package.json


---

## ⚙️ API Endpoints

### 🔹 Track User Event
POST /api/events

Request Body:
{
  "userId": "123",
  "eventType": "login",
  "timestamp": "2026-04-18T10:00:00Z"
}
🔹 Get Analytics

GET /api/analytics

Response Example:

{
  "dailyActiveUsers": 120,
  "mostFrequentEvent": "login"
}

⏱️ Automated Reports
Daily reports generated using node-cron
Includes:
Total users
Event distribution
Activity trends

