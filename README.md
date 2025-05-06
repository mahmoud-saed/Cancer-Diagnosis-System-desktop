# Cancer Diagnosis System Desktop

A cross-platform desktop application designed to assist in cancer diagnosis, leveraging a modern tech stack with **Electron.js** for the frontend and **Django** for the backend.

---

## 📋 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)
- [Contributors](#contributors)
- [License](#license)

---

## 🧠 Introduction

The **Cancer Diagnosis System Desktop** application aims to provide a user-friendly interface for medical professionals to input patient data and receive diagnostic insights. By integrating Electron.js and Django, the application ensures a seamless experience across different operating systems.

---

## ✨ Features

- **Cross-Platform Compatibility**: Runs smoothly on Windows, macOS, and Linux.
- **Modern UI**: Built with Electron.js to provide a responsive and intuitive user interface.
- **Robust Backend**: Utilizes Django to handle data processing and business logic.
- **Modular Architecture**: Clean separation between frontend and backend components for maintainability.

---

## 🛠️ Installation

### Prerequisites

- **Node.js**: Ensure you have Node.js installed for the Electron frontend.
- **Python 3.x**: Required for the Django backend.
- **pip**: Python package installer.
- **virtualenv** (optional but recommended): For creating isolated Python environments.

### Steps

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/mahmoud-saed/Cancer-Diagnosis-System-desktop.git
   cd Cancer-Diagnosis-System-desktop
   ```


2. **Setup Backend**:

   ```bash
   cd Back-end
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   python manage.py migrate
   python manage.py runserver
   ```


3. **Setup Frontend**:

   ```bash
   cd ../Front-end
   npm install
   npm start
   ```


---

## 🚀 Usage

1. **Start the Django Backend**:

   ```bash
   cd Back-end
   python manage.py runserver
   ```


2. **Launch the Electron Frontend**:

   ```bash
   cd ../Front-end
   npm start
   ```


3. **Interact with the Application**:

   Use the Electron interface to input patient data and view diagnostic results.

---

## 📁 Project Structure


```plaintext
Cancer-Diagnosis-System-desktop/
├── Back-end/
│   ├── manage.py
│   ├── requirements.txt
│   └── ... (Django project files)
├── Front-end/
│   ├── package.json
│   ├── main.js
│   └── ... (Electron project files)
└── README.md
```


---

## 📦 Dependencies

### Backend (Django)

- Django==3.x.x
- djangorestframework==3.x.x
- ... (other dependencies as listed in `requirements.txt`)

### Frontend (Electron)

- Electron==x.x.x
- ... (other dependencies as listed in `package.json`)

---

## ⚙️ Configuration

- **Backend**: Configure Django settings in `Back-end/settings.py` as needed.
- **Frontend**: Modify Electron configurations in `Front-end/main.js` or related files.

---

## 🐞 Troubleshooting

- **Port Conflicts**: Ensure that the ports used by Django and Electron are not occupied by other applications.
- **Dependency Issues**: Verify that all dependencies are correctly installed and compatible with your system.
- **Cross-Origin Requests**: If encountering CORS issues, configure Django's CORS settings accordingly.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
