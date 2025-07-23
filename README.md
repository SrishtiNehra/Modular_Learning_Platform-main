# 📚 Modular Learning Platform (MERN Stack Assignment)

A scalable, modular e-learning platform designed to provide structured course experiences with interactive learning, user progress tracking, and a role-based content management system.

> 🧠 Built with **MongoDB, Express, React (Next.js), and Node.js**  
> 🔐 Role-based authentication using **JWT**  
> 🧩 Nested learning structure: Courses → Sections → Units → Chapters

---

##  Project Overview

This learning platform allows:
- 👨‍🏫 **Admins** to create and manage modular course content
- 👨‍🎓 **Learners** to enroll, explore, and interact with educational material

🕒 **Estimated Time to Complete**: 3–4 Days

---

## ✅ Features

### 1. 🔐 Authentication & Authorization
- JWT-based secure login and registration
- Two user roles: `admin`, `learner`
- Role-based protected routes and dashboards

### 2. 🧱 Course Hierarchy & Management (Admin Panel)
- **CRUD Operations** for:
  - Courses
  - Sections under each course
  - Units under each section
  - Chapters under each unit
- Chapter-level interactive questions:
  - MCQs
  - Fill in the blanks
  - Text-based responses
  - 🎤 Audio-based answers (bonus)
- Support for question metadata:
  - Question text
  - Options (if applicable)
  - Correct answer
  - Media (optional image/audio)

### 3. 📖 Learning Experience (Learner Panel)
- Dashboard to view and continue enrolled courses
- Real-time progress saving at section/unit/chapter level
- Attempt and review chapter questions
- Get instant score summary upon completing chapters

---

## 🛠️ Tech Stack

| Layer       | Technology            |
|-------------|------------------------|
| Frontend    | **Next.js (React)**    |
| Backend     | **Node.js + Express**  |
| Database    | **MongoDB + Mongoose** |
| Auth        | **JWT**                |
| State Mgmt  | **React Context / Redux** |

---

## 🧩 Database Schema (Models)

- **User**: name, email, role (`admin`, `learner`), password hash
- **Course** → **Section** → **Unit** → **Chapter**
- **Question**: type, text, options, correct answer, media
- **UserProgress**: userId, courseId, lastProgress (section/unit/chapter)

---

## 🧪 API Features

- Clean RESTful API design using Express
- Nested `populate()` logic for Course hierarchy
- Input validation, error handling, and request sanitization

---

## 💻 Frontend Highlights

- Dynamic routing and SSR/SSG using **Next.js**
- Responsive and role-based dashboards
- Accordion/Tree UI for nested learning structure
- Progress tracking stored in state and synced with backend

---

## 📂 Folder Structure (Suggested)

```

root/
├── Frontend/              # Next.js frontend
│   └── components/
│   └── pages/
│   └── context/
│   └── utils/
├── Backend/              # Express backend
│   └── controllers/
│   └── models/
│   └── routes/
│   └── middleware/
│   └── config/
├── .env
├── README.md
└── package.json

```

## 📌 Future Enhancements

- Role management panel for admins
- Media uploads via Cloudinary
- Leaderboards or gamification
- Real-time collaboration in learning

---

## 🧑‍💻 Author

**Umesh Rao**  
GitHub: [@umeshyadav7988](https://github.com/umeshyadav7988)

---

---

```

