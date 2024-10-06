

# **Center for Comparative Archaeology - Database Management System**

In the realm of archaeological research and resource management, the **Center for Comparative Archaeology** website is designed to facilitate seamless access, contribution, and management of archaeological databases. The platform offers a user-friendly interface, enabling users to download existing datasets and actively contribute to their growth. 

This project aims to create an accessible hub for managing, contributing to, and disseminating archaeological data. Built using **Python Flask, MySQL, SQLAlchemy, HTML, and CSS**, the system allows users to view, download, and contribute to datasets, while also requesting new project creation after registering.

---

## **Key Features**

### **Guest Access**:
- View and download existing archaeological datasets in **Excel** and **CSV** formats.

### **Registered User Access**:
- Submit requests to create new projects.
- Contribute to existing projects by uploading Excel sheets with the same structure.
- View your profile, showcasing previous projects and research interests.

### **Moderator Dashboard**:
- Review and approve requests submitted by registered users (e.g., creating new projects or contributing to existing ones).

---

## **System Requirements**

### **1. Web Server**
- **Flask** web framework for Python with **Werkzeug** as the WSGI server.
- Deployment on a server capable of handling Flask applications (e.g., **Gunicorn**, **uWSGI**).
- Option to configure a reverse proxy (e.g., **Nginx**, **Apache**) for enhanced security and performance.

### **2. Database Management System**
- **MySQL 8.0** for efficient data storage and retrieval.
- **Flask-SQLAlchemy** for simplified database interactions within the Flask application.
- Proper database schema design to support user profiles, notifications, contributions, and moderation logs.

### **3. Programming Languages**
- **Python 3.7** or later for server-side scripting with Flask.
- **HTML5, CSS3, JavaScript** for front-end development.
- **Jinja2** for integrating Python with HTML templates.

### **4. User Authentication & Security**
- **Flask-Security** for user authentication and authorization.
- Secure password hashing using libraries like **Werkzeug**.
- Protection against common web vulnerabilities through Flask extensions and input validation.

### **5. User Interface Compatibility**
- **Responsive design** with HTML5 and CSS3 for optimal viewing on various devices.
- **JavaScript** for client-side interactivity.

### **6. Notification System**
- **Flask-SocketIO** for real-time updates through WebSocket functionality.
- Integration with **Flask-Mail** for email notifications.

### **7. User Management**
- **Flask-Login** for managing user sessions.
- User registration and profile management via Flask forms.
- Account deletion functionality with data retention policies.

### **8. Moderation Tools**
- Custom moderation interfaces or **Flask-admin** panel for reviewing user submissions.
- Logging moderator activities within the Flask application.

### **9. File Management**
- **Flask-Uploads** for secure file upload and management.
- File type verification to maintain the integrity of contributed content.

### **10. Compatibility Testing**
- Cross-browser compatibility testing (Chrome, Firefox, Safari).
- Responsive design testing across devices and screen resolutions.

### **11. Documentation & Help System**
- Comprehensive documentation for developers on setting up, configuring, and maintaining the application.
- In-app help system or separate knowledge base for user assistance.

### **12. Backup & Recovery**
- Automated database backups using tools like **mysqldump**.
- A well-defined disaster recovery plan to minimize data loss and downtime.

---

## **Dependencies**

The following dependencies must be installed in a virtual environment:

- **Flask**
- **Flask-WTF**
- **Flask-SQLAlchemy**
- **Pandas**
- **MySQL Connector for Python**
- **Phonenumbers**
- **Flask-Login**
- **WTForms-Alchemy**

---

## **Installation Steps**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   ```

2. Navigate to the project directory:
   ```bash
   cd your-repo
   ```

3. Create a virtual environment:
   ```bash
   python3 -m venv dbenv
   ```

4. Activate the virtual environment:
   - On macOS/Linux:
     ```bash
     source dbenv/bin/activate
     ```
   - On Windows:
     ```bash
     dbenv\Scripts\activate
     ```

5. Install dependencies:
   ```bash
   pip install Flask Flask-WTF Flask-SQLAlchemy pandas mysql-connector-python phonenumbers Flask-Login wtforms-alchemy
   ```

6. Set Flask environment variables:
   ```bash
   export FLASK_ENV=development
   export FLASK_APP=script.py
   ```

7. Run the application:
   ```bash
   flask run
   ```

8. Access the application in your browser at:
   ```
   http://127.0.0.1:5000
   ```
