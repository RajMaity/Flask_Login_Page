# Flask Login & Registration System

A lightweight, functional Flask web application that demonstrates user registration, session-based authentication, and protected routing.

## 🚀 Features
* **User Registration:** Allows new users to sign up and stores data in a local dictionary.
* **Secure Sessions:** Uses Flask Sessions to keep users logged in across different pages.
* **Flash Messaging:** Integrated feedback system for login errors and successful registrations (Success, Danger, and Warning alerts).
* **Protected Routes:** The `/home` dashboard is protected; unauthorized users are automatically redirected to the login page.
* **Logout Functionality:** Properly clears session data to secure user accounts.

---

## 🛠️ Installation & Setup

### 1. Clone the repository
```bash
git clone [https://github.com/RajMaity/Flask_Login_Page.git](https://github.com/RajMaity/Flask_Login_Page.git)
cd Flask_Login_Page

2. Create a Virtual Environment (Recommended)
Bash

# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
Bash

pip install flask
4. Run the Application
Bash

python app.py
The app will be live at http://127.0.0.1:5000/.

📂 Project Structure
Plaintext

.
├── app.py              # Main Flask application logic & routing
├── templates/
│   ├── login.html        # Login form UI
│   ├── registration.html # Signup form UI
│   └── home.html         # User dashboard (Protected)
└── README.md
📝 Important Notes
Data Persistence
This application currently uses an in-memory dictionary (credentials_dict) to store users.

Note: Because data is stored in a Python dictionary, all registered users will be deleted whenever the Flask server restarts.

Security
Secret Key: The app.secret_key is hardcoded for demonstration. In a production environment, this should be stored in an environment variable.

Password Storage: Currently, passwords are stored in plain text. For production apps, always use a library like Werkzeug or Bcrypt to hash passwords.

👤 Author
Raj Maity

GitHub: @RajMaity

Future Enhancements
[ ] Add SQLite/PostgreSQL database support for permanent storage.

[ ] Implement Password Hashing for security.

[ ] Add CSS styling (Bootstrap) to the HTML templates.
