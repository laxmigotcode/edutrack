 # EduTrack — Student Registration & Records Portal

A modern, fast, and accessible student registration web application built with clean **HTML5, CSS3, and Vanilla JavaScript**.

Designed with beginner-friendly architecture: **zero configuration**, **no build steps**, and **no external dependencies**.

---

## 🚀 How to Run the Website

Because this project is built using standard web technologies, you don't need to install Node.js, Python, or any packages to run it.

### Option 1: Direct File Launch (Easiest)
1. Navigate to the project folder on your computer:
   `c:\Users\laksh\Desktop\website\student registration`
2. **Double-click `index.html`**.
3. It will immediately open and run in your default web browser (Chrome, Edge, Firefox, Brave, Safari).

### Option 2: Using VS Code Live Server (Recommended for Learning)
1. Open the project folder in VS Code.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click `index.html` and select **"Open with Live Server"**.
4. The site will open at `http://127.0.0.1:5500/index.html` and automatically refresh whenever you edit code!

### Option 3: Using Python (Optional Local Server)
If you have Python installed, open PowerShell in this directory and run:
```powershell
python -m http.server 8000
```
Then visit `http://localhost:8000` in your browser.

---

## 📁 Project Architecture & File Guide

```text
student registration/
├── index.html            # Main HTML document (Semantic tags, tabs, form, table, modals)
│
├── css/
│   ├── styles.css        # Base theme, CSS variables, typography, layout, & responsive media queries
│   └── components.css    # Reusable components: cards, buttons, form inputs, table, modals, & toast alerts
│
├── js/
│   ├── storage.js        # Data layer: CRUD operations (get, add, update, delete, seed) using localStorage
│   ├── validation.js     # Form validation rules (names, emails, phones, duplicate roll numbers)
│   └── app.js            # Main controller: DOM interactions, tab switching, and CSV export
│
└── assets/
    └── default-avatar.svg # Vector avatar placeholder when no student picture is uploaded
```

---

## ✨ Features Breakdown

- **Real-Time Form Validation**:
  - Validates full name, email format, phone numbers (10–15 digits), and date of birth (enforcing a minimum age of 14).
  - Checks student ID/Roll Number uniqueness to prevent duplicate registrations.
  - Highlights invalid fields with red borders and clear error descriptions.
- **Profile Photo Upload & Preview**:
  - Live preview when choosing an image.
  - Automatically converted to Base64 and stored with the student's profile.
  - Fallback SVG avatar if no photo is uploaded.
- **Local Data Persistence (`localStorage`)**:
  - All records remain saved in your browser even if you refresh or close the tab.
- **Search & Filter Controls**:
  - Instant as-you-type search across names, IDs, and email addresses.
  - Filter by Department or Academic Year.
- **Full CRUD Support**:
  - **Create**: Register new students with rich details.
  - **Read**: View directory table or click 👁️ "View" for a full-screen profile card.
  - **Update**: Click ✏️ "Edit" to load student data back into the form and save changes.
  - **Delete**: Click 🗑️ to trigger a safe confirmation dialog before removing a record.
- **Testing & Utility Tools**:
  - **⚡ Load Sample Data**: Pre-populates 4 realistic students with a single click.
  - **📥 Export to CSV**: Downloads all records into an Excel-compatible spreadsheet file.
- **Accessibility & Responsiveness**:
  - Fully responsive across mobile (375px), tablet (768px), and desktop (1200px+).
  - Accessible `<label>` pairings, ARIA roles, focus visible rings, and screen-reader considerations.
