# 🎓 Internship Tracker — Full Stack

A beautiful full-stack internship tracking platform built with **pure Node.js** (zero npm dependencies!) and a gorgeous dark UI.

---

## 🚀 Quick Start

```bash
# 1. Go to the project folder
cd internship-tracker

# 2. Start the server (no npm install needed!)
node server.js

# 3. Open your browser
# → http://localhost:3000
```

---

## 🔐 Default Logins

| Role    | Email / Username         | Password     |
|---------|--------------------------|--------------|
| Admin   | `admin`                  | `1234`       |
| Student | `student@college.edu`    | `student123` |

---

## 📁 Project Structure

```
internship-tracker/
├── server.js          ← Backend (pure Node.js, no npm)
├── public/
│   └── index.html     ← Frontend (HTML + CSS + JS)
└── data/              ← JSON database (auto-created)
    ├── users.json
    ├── internships.json
    ├── profiles.json
    ├── notes.json
    ├── calendar.json
    └── notices.json
```

---

## 🔧 API Endpoints

### Auth
| Method | Endpoint             | Description         |
|--------|----------------------|---------------------|
| POST   | `/api/auth/login`    | Login               |
| POST   | `/api/auth/register` | Student register    |
| GET    | `/api/auth/me`       | Get current user    |

### Internships
| Method | Endpoint                     | Description         |
|--------|------------------------------|---------------------|
| GET    | `/api/internships`           | Get all             |
| POST   | `/api/internships`           | Add new             |
| PUT    | `/api/internships/:id`       | Edit (admin)        |
| DELETE | `/api/internships/:id`       | Delete (admin)      |

### Other
| Method | Endpoint         | Description     |
|--------|------------------|-----------------|
| GET/PUT | `/api/profile`  | Student profile |
| GET/POST | `/api/notes`   | Notes           |
| GET/POST | `/api/calendar`| Calendar dates  |
| GET/POST | `/api/notices` | Admin notices   |
| GET    | `/api/stats`     | Stats summary   |
| GET    | `/api/admin/users` | All users (admin) |

---

## ✨ Features

- **JWT Authentication** (custom, no library)
- **Role-based access** (Admin / Student)
- **File-based JSON database** (no MongoDB needed)
- **Student self-registration**
- **Internship CRUD** with search & filter
- **Profile with photo**
- **Notes** persisted to server
- **Calendar** dates saved
- **Admin notice board**
- **Interview quiz** with progress tracker
- **CSV Export**
- **Live API status** badge in UI

---

## 🔒 Security

- Passwords hashed with HMAC-SHA256
- JWT tokens for session management
- Role-based route protection
- Students can only see their own data

---

Built with ❤️ — Pure Node.js, zero dependencies
