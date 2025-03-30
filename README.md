# 📚 E-Notes Management System

## 📌 Introduction
The **E-Notes Management System** is a web-based platform that allows users (students, teachers, and admins) to upload, organize, and share notes securely. The system ensures efficient document management, categorization, and collaboration.

## 🚀 Features
### 🎓 User Management
- 🔑 **JWT Authentication** – Secure login/logout with role-based access (Student, Teacher, Admin)
- 📌 **Profile Management** – Users can update their details and manage account settings
- 🏷 **Role-Based Access Control (RBAC)** – Different access levels for managing and sharing notes

### 📄 Notes Management
- 📤 **Upload Notes** – Supports various formats (PDF, DOCX, TXT, Images)
- 🗂 **Categorize Notes** – Organize notes under subjects, topics, or custom categories
- 🏷 **Tagging System** – Add tags for better searching and filtering
- 🖊 **Edit & Delete Notes** – Users can modify or remove their uploaded notes

### 🔄 Notes Sharing & Collaboration
- 🔗 **Share Notes via Links** – Generate shareable links for specific notes
- 🔒 **Access Control** – Set permissions (Public, Private, or Specific Users)
- 💬 **Commenting & Feedback** – Users can comment on shared notes

### 📊 Reports & Analytics
- 📈 **Dashboard Overview** – View recent uploads, most viewed/downloaded notes
- 📊 **User Activity Logs** – Track logins, uploads, and sharing history

### 📩 Notifications & Alerts
- 📢 **New Notes Alerts** – Notify users when new notes are added in their categories
- ⏳ **Reminders** – Remind users about pending approvals or unread notes
- ⚠ **Security Alerts** – Notify admins about suspicious activities

## 🏗 Project Structure
```
enotes_management/
│── backend/                      # Django Backend
│   ├── Enotes_Management_System/                    # Main Django Project
│   │   ├── settings.py            # Project settings
│   │   ├── urls.py                # Project URL configuration
│   │   ├── wsgi.py                # WSGI entry point
│   │   ├── asgi.py                # ASGI entry point (optional)
│   │   ├── manage.py              # Django management script
│   │
│   ├── enotes/                      # Django Apps
│   │   ├── __init_.py/        
│   │   ├── admin.py/                
│   │   ├── apps.py/
│   │   ├── models.py/              
│   │   ├── tests.py/       
│   │   ├── views.py/             
│   │
│   ├── static/                    # Static Files (CSS, JS, images)
│   ├── media/                     # Uploaded Files (PDFs, Docs, Images)
│   ├── templates/                 # Django Templates
│
```

## 🔧 Installation & Setup
### 1️⃣ Prerequisites
Ensure you have the following installed:
- **Python 3.x** (For Django backend)
- **PostgreSQL/MySQL** (Database)


### 2️⃣ Clone the Repository
```
git clone https://github.com/NandiniReddy9/E-Notes-Management.git
cd enotes-management
```

### 3️⃣ Set Up Virtual Environment & Install Dependencies
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables
Create a `.env` file in the backend directory:
```
SECRET_KEY=your-secret-key
DEBUG=True
DATABASE_URL=postgres://username:password@localhost:5432/enotes
JWT_SECRET=your-jwt-secret
```

### 5️⃣ Run Migrations & Start the Server
```
python manage.py migrate
python manage.py runserver
```

### 6️⃣ Run Frontend (Optional for React)
```
cd frontend
npm install
npm start
```

## 🖥 API Endpoints
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | `/api/auth/register/` | Register a new user |
| POST | `/api/auth/login/` | Login user & get token |
| GET | `/api/notes/` | Retrieve all notes |
| POST | `/api/notes/upload/` | Upload a new note |
| PATCH | `/api/notes/{id}/` | Edit a note |
| DELETE | `/api/notes/{id}/` | Delete a note |
| POST | `/api/notes/share/` | Share a note |

## 📌 Status Codes
| Status Code | Meaning |
|------------|---------|
| 200 OK | Request was successful |
| 201 Created | New resource created |
| 400 Bad Request | Invalid input |
| 401 Unauthorized | Authentication failed |
| 403 Forbidden | Access denied |
| 404 Not Found | Resource not found |
| 500 Internal Server Error | Server issue |

## 🔒 Security
- **JWT Authentication** for secure API access
- **Role-based access control (RBAC)**
- **Data Encryption** for user data & notes
- **Logging & Monitoring** for tracking activities

## 🚀 Deployment Guide
### 1️Setup & Configure the Environment
Modify `.env` with production credentials.




## 🤝 Contributing
Contributions are welcome! Follow these steps:
1. Fork the repository
2. Create a new branch (`feature-new`)
3. Commit your changes
4. Push to your fork and submit a pull request

## 📞 Contact & Support
- 📧 Email: support@enotes.com
- 📖 Documentation: [API Docs](https://api.enotes.com/docs)
- 🌐 Website: [www.enotes.com](https://www.enotes.com)



---

### 💡 Happy Coding! 🚀

