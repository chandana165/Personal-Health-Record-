# 🩺 PHR Vault — Personal Health Record Manager

A secure, web-based **Personal Health Record (PHR)** application built with **Flask**, letting users store, organize, and retrieve their medical information and documents in one place.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-black?logo=flask)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57?logo=sqlite&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)

---

## 📌 Overview

Medical records are often scattered across hospitals, labs, and paper files. **PHR Vault** gives individuals a single, private place to manage their own health data.

> **Problem:** Health records are fragmented and hard to access when needed.
> **Solution:** A centralized, user-owned vault with authentication, structured records, and document uploads.

## ✨ Features

<!-- Edit this list so it matches exactly what your app does -->
- 🔐 User registration & secure login (hashed passwords)
- 📋 Add, view, edit, and delete health records
- 📎 Upload and store medical documents (reports, prescriptions, scans)
- 🗂️ Organized, searchable record history
- ✅ Server-side form validation (Flask-WTF)
- 🗄️ Database versioning with migrations

## 🛠️ Tech Stack

| Layer      | Technology                              |
|------------|-----------------------------------------|
| Backend    | Python, Flask                           |
| Database   | SQLite, SQLAlchemy ORM, Flask-Migrate   |
| Forms      | Flask-WTF / WTForms                     |
| Frontend   | HTML, CSS, JavaScript (Jinja2 templates)|

## 📁 Project Structure

```
Personal-Health-Record-/
├── app.py              # Application entry point & routes
├── config.py           # App configuration
├── models.py           # Database models
├── forms.py            # Form definitions & validation
├── utils.py            # Helper functions
├── migrations/         # Database migrations
├── templates/          # Jinja2 HTML templates
├── static/             # CSS, JS, images
├── uploads/            # User-uploaded files (git-ignored)
└── requirements.txt    # Python dependencies
```

## 🚀 Getting Started

### Prerequisites
- Python 3.10 or higher
- pip

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/chandana165/Personal-Health-Record-.git
cd Personal-Health-Record-

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set up the database
flask db upgrade

# 5. Run the app
python app.py
```

Then open **http://127.0.0.1:5000** in your browser.

### Environment Variables

Create a `.env` file (never commit it):

```
SECRET_KEY=your-random-secret-key
```

## 📸 Screenshots

<!-- Add 3–4 screenshots to a /screenshots folder, then uncomment -->
<!--
| Login | Dashboard |
|-------|-----------|
| ![Login](screenshots/login.png) | ![Dashboard](screenshots/dashboard.png) |
-->

## 🔒 Security & Privacy

- Passwords are stored hashed, never in plain text
- Secrets are loaded from environment variables
- Uploaded files and the local database are excluded from version control

## 🗺️ Roadmap

- [ ] Role-based access (patient / doctor)
- [ ] Appointment & medication reminders
- [ ] Export records as PDF
- [ ] Deploy to a cloud platform
- [ ] Unit tests & CI with GitHub Actions

## 🤝 Contributing

Suggestions and pull requests are welcome. Open an issue to discuss any major change first.

## 👩‍💻 Author

**Chandana**
- GitHub: [@chandana165](https://github.com/chandana165)
- LinkedIn: [linkedin.com/in/b-v-chandana-b528112b3]
- Email: [chandanabv26@gmail.com]

## 📄 License

This project is licensed under the MIT License — see the `LICENSE` file for details.
