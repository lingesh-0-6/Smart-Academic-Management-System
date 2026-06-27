# 🎓 Smart Academic Management System (SAMS)

A full-stack academic management platform that integrates an Institute Management System (IMS), Moodle-inspired Learning Management System, and an intelligent Email Event Detection service into one unified ecosystem.

## 🚀 Overview

Smart Academic Management System (SAMS) is designed to simplify academic management by centralizing assignments, academic events, and reminders in a single platform.

Unlike traditional systems where students must manually check multiple portals and emails, SAMS automatically detects academic events from college emails, displays them in an integrated calendar, and allows students to receive personalized WhatsApp reminders.

---

## ✨ Key Features

### 📚 Institute Management System (IMS)
- Student Dashboard
- Academic Calendar
- Event Management
- Smart Reminder System
- WhatsApp Notifications

### 📖 Moodle Module
- Faculty Login
- Student Login
- Course Management
- Assignment Creation
- Assignment Submission
- Submission Tracking

### 📩 Email Integration
- Gmail API Integration
- OAuth 2.0 Authentication
- Automatic Email Fetching
- Event Detection
- Rule-based NLP
- Calendar Event Creation

### 📲 Smart Reminder System
- "Remind Me" feature
- WhatsApp reminders using Twilio
- Reminder sent:
  - 2 days before registration deadline
  - OR 2 days before event date if no registration deadline exists

---

# 🏗️ Project Structure

```
Smart-Academic-Management-System
│
├── rit-ims-v2
│   ├── frontend
│   └── backend
│
├── moodle
│   ├── frontend
│   └── backend
│
├── email-integration
│
└── README.md
```

---

# 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- CSS Modules

### Backend
- Node.js
- Express.js

### Database
- MySQL

### APIs
- REST API
- Fetch API

### Authentication
- Google OAuth 2.0

### Email Processing
- Gmail API

### Notifications
- Twilio WhatsApp API

### Scheduling
- Node Cron

### NLP
- Rule-based Keyword Matching

---

# 🔄 System Workflow

```
College Gmail
      │
      ▼
Email Integration Service
      │
      ▼
Event Detection (NLP)
      │
      ▼
Shared MySQL Database
      │
      ├─────────────► IMS Calendar
      │
      ├─────────────► Moodle
      │
      ▼
Reminder Engine
      │
      ▼
Twilio WhatsApp API
      │
      ▼
Student
```

---

# 📂 Modules

## 1️⃣ IMS
Handles:
- Dashboard
- Calendar
- Events
- Reminders

---

## 2️⃣ Moodle
Handles:
- Assignments
- Courses
- Faculty
- Students

---

## 3️⃣ Email Integration
Handles:
- Gmail Authentication
- Email Reading
- Event Detection
- Database Updates
- Reminder Scheduling

---

# 🔐 Environment Variables

Create `.env` files using the provided `.env.example` templates.

Required services:

- MySQL
- Google Cloud OAuth Credentials
- Gmail API
- Twilio Account

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/lingesh-0-6/Smart-Academic-Management-System.git
```

Install dependencies inside each project.

Example:

```bash
cd rit-ims-v2/backend
npm install
```

Repeat for:

- rit-ims-v2/frontend
- moodle/backend
- moodle/frontend
- email-integration

---

# ▶️ Running the Project

Start each service separately.

IMS Backend

```bash
npm start
```

IMS Frontend

```bash
npm run dev
```

Moodle Backend

```bash
npm start
```

Moodle Frontend

```bash
npm run dev
```

Email Integration

```bash
node server.js
```

---

# 💡 Future Enhancements

- AI-based Event Prioritization
- Mobile Application
- Cloud Deployment
- Push Notifications
- OCR Support for Posters
- Multi-College Support

---

# 👨‍💻 Team

Developed as a Hackathon Project by

- Lingesh
- Keerthana

---

# 📄 License

This project is intended for educational and demonstration purposes.
