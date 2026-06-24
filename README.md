# 💼 JobOps – Job Application Portal

A Full‑Stack Job Application Portal built as part of a Database Management System (DBMS) course. JobOps allows users to browse job listings, apply with a resume and profile photo, save jobs, track applications, and manage their account – all wrapped in a clean, responsive interface.

<p align="center">
  <img src="Demo_Media/WebAppLogo.png" alt="JobOps Dashboard" width="700"/>
</p>

---

## 📑 Table of Contents

- [✨ Features](#-features)
- [🖼️ Screenshots](#️-screenshots)
- [⚙️ Tech Stack](#️-tech-stack)
- [📁 Folder Structure](#-folder-structure)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [🎬 Demo Video](#-demo-video)
- [🐛 Troubleshooting](#-troubleshooting)
- [📄 License](#-license)
- [📫 Contact](#-contact)

---

## ✨ Features

- **User Authentication** – Register, login, change password, delete account.
- **Job Browsing** – View all job postings with filters and search.
- **Application Management** – Apply to jobs, upload resume and profile photo.
- **Saved Jobs** – Bookmark jobs for later.
- **Profile Management** – Update personal details and uploaded documents.
- **Admin Panel** – (Optional) manage job listings and users.
- **Responsive UI** – Works on desktop and mobile devices.

---

## 🖼️ Screenshots

All screenshots are located in the [`Demo_Media/`](Demo_Media) folder.

<p align="center">
  <table>
    <tr>
      <td align="center">
        <img src="Demo_Media/AboutPage.png" alt="AboutPage" width="300"/><br/>
        <sub>About Page</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/ApplicationPage.png" alt="ApplicationPage" width="300"/><br/>
        <sub>Application Page</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/AppliedJobs.png" alt="AppliedJobs" width="300"/><br/>
        <sub>Applied Jobs</sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="Demo_Media/ChangePassword.png" alt="ChangePassword" width="300"/><br/>
        <sub>Change Password</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/ContactPage1.png" alt="ContactPage1" width="300"/><br/>
        <sub>Contact Page Upper</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/ContactPage2.png" alt="ContactPage2" width="300"/><br/>
        <sub>Contact Page Lower</sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="Demo_Media/DeleteAccount.png" alt="DeleteAccount" width="300"/><br/>
        <sub>Delete Account</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/JobDescription.png" alt="JobDescription" width="300"/><br/>
        <sub>Job Description</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/JobFilterPage.png" alt="JobFilterPage" width="300"/><br/>
        <sub>Job Filter Page</sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="Demo_Media/MainPage1.png" alt="MainPage1" width="300"/><br/>
        <sub>Main Page Upper</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/MainPage2.png" alt="MainPage2" width="300"/><br/>
        <sub>Main Page Lower</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/ProfilePage.png" alt="ProfilePage" width="300"/><br/>
        <sub>Profile Page</sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="Demo_Media/RegistrationPage.png" alt="RegistrationPage" width="300"/><br/>
        <sub>Registration Page</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/LoginPage.png" alt="LoginPage" width="300"/><br/>
        <sub>Login Page</sub>
      </td>
      <td align="center">
        <img src="Demo_Media/SavedJobs.png" alt="SavedJobs" width="300"/><br/>
        <sub>Saved Jobs</sub>
      </td>
    </tr>
  </table>
</p>

---

## ⚙️ Tech Stack

| **Layer** | **Technologies** |
|-----------|-------------------|
| **Frontend** | React.js, Vite, Tailwind CSS, Axios |
| **Backend** | Node.js, Express.js, Multer, JWT, bcrypt |
| **Database** | PostgreSQL, MongoDB, Cloudinary API |
| **File Storage** | Local File System and Cloudinary Image Store |
| **Build Tools** | npm, nodemon, nvm |

---

## 📁 Folder Structure

```
JobOps-Project/
|
├── Backend/                 
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── uploads/             
│   ├── server.js
│   ├── app.js
│   ├── .gitignore
│   ├── package-lock.json
│   └── package.json
|
├── Frontend/                
│   ├── public/
│   ├── src/
│   ├── .eslintrc.cjs
│   ├── .gitignore
│   ├── index.html
│   ├── package-lock.json
│   ├── package.json
│   ├── postcss.config.js
│   ├── README.md
│   ├── tailwind.config.js
│   ├── vercel.json
│   └── vite.config.js
|
├── Demo_Media/      
│   ├── AboutPage.png
│   ├── ApplicationPage.png        
│   ├── AppliedJobs.png
│   ├── ChangePassword.png
│   ├── ContactPage1.png
│   ├── ContactPage2.png
│   ├── DBMS_Project_Preview.mp4
│   ├── DeleteAccount.png
│   ├── JobDescription.png
│   ├── JobFilterPage.png
│   ├── LoginPage.png
│   ├── MainPage1.png
│   ├── MainPage2.png
│   ├── ProfilePage.png
│   ├── RegistrationPage.png
│   ├── SavedJobs.png
│   └── WebAppLogo.png
|
├── Test_Images/             
│   ├── SampleProfilePhoto.jpg
│   └── SampleResume.pdf
|
└── README.md (This File)
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v22 or later, use "nvm" if needed) and **npm** installed.
- **MongoDB** installed and running locally (use "mongod" command in terminal).
- A code editor (VS Code recommended).

---

### Backend Setup

1. **Navigate to the Backend folder:**
   ```bash
   cd Backend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create environment configuration:**
   - Copy `config/config.sample.env` → `config/config.env`.
   - Fill in your database credentials and JWT secret.

4. **Set up the database:**
   - Create a PostgreSQL database (e.g., `jobops`).
   - Run the SQL scripts (provided in `config/db.sql` if available) to create tables.

5. **Start the backend server:**
   ```bash
   node server.js
   ```
   The server will run on `http://localhost:5000` (or the port you set).

---

### Frontend Setup

1. **Navigate to the Frontend folder:**
   ```bash
   cd Frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure API base URL:**
   - Edit the `.env` file (or directly in `src/api.js`) to point to your backend URL.

4. **Run the development server:**
   ```bash
   npm run dev
   ```
   The frontend will be available at `http://localhost:5173`.

---

> **Note:** If you encounter dependency issues, try `npm audit fix` or `npm audit fix --force`.

---

## 🎬 Demo Video

Watch the full walkthrough on YouTube: 

[![JobOps Demo](https://img.youtube.com/vi/wZ9ENq3zazA/0.jpg)](https://youtu.be/wZ9ENq3zazA)

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| **Port conflict** | Change the port in `config.env` (backend) or `vite.config.js` (frontend). |
| **Database connection fails** | Verify your PostgreSQL credentials and ensure the service is running. |
| **Uploads not working** | Check that the `uploads/` folder exists and has write permissions. |
| **Missing environment variables** | Ensure `config.env` is present and contains all required keys. |
| **npm install errors** | Use `npm install --legacy-peer-deps` if you face dependency conflicts. |

---

## 📄 License

This project is for educational purposes. Feel free to use and modify it for your own learning.

---

## 📫 Contact

For questions, suggestions, or collaborations, reach out via [GitHub](https://github.com/Kratugautam99) or leave a comment on the demo video.

---

<p align="center">
  <strong>♦️ Happy Job Hunting!</strong>
</p>
