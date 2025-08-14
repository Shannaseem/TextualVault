TextualVault
TextualVault is a Python-based application that combines a Textual User Interface (TUI) with backend logic for data storage, email utilities, and user management.It is built using Python, SQLAlchemy for database operations, and the textual TUI framework.

📂 Project Structure
TextualVault/
├── app/
│ ├── **init**.py # Package initializer
│ ├── crud.py # Create, Read, Update, Delete operations
│ ├── database.py # Database connection and session management
│ ├── email_utils.py # Functions for sending and handling emails
│ ├── main.py # Main backend entry point
│ ├── models.py # SQLAlchemy models for database tables
│ ├── tui_main.py # Text-based User Interface entry point
├── .gitignore # Git ignore rules
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── .env # Environment variables (ignored by Git)

Note: The .env file contains sensitive information and is ignored by Git for security.

🚀 Features

Database Support: SQLAlchemy ORM for efficient data storage and retrieval.
Email Utilities: Send OTPs and notifications via configurable SMTP.
Textual UI: Interactive command-line interface using the textual framework.
Modular Design: Separated modules for CRUD operations, database models, and UI.
Environment Configuration: Securely manage API keys, database credentials, and email settings via .env.

🛠 Installation
Prerequisites

Python 3.8 or higher
PostgreSQL (for database support)
A valid SMTP server account for email functionality
git for cloning the repository

Steps

Clone the repository
git clone https://github.com/Shannaseem/TextualVault.git
cd TextualVault

Create and activate a virtual environment
python -m venv .venv

# Linux/Mac

source .venv/bin/activate

# Windows

.venv\Scripts\activate

Install dependencies
pip install -r requirements.txt

Set up environment variables
Create a .env file in the project root with the following (replace with your values):
DATABASE_URL=postgresql+psycopg2://user:password@localhost:5432/textualvault
EMAIL_HOST=smtp.example.com
EMAIL_PORT=587
EMAIL_USER=your_email@example.com
EMAIL_PASSWORD=your_email_app_password

▶ Usage

Run the backend logic
python -m app.main

Run the TUI application
python -m app.tui_main

🔐 Security Precautions

Never commit .env to GitHub as it contains sensitive credentials.

Ensure .gitignore includes:
.env
.venv/
**pycache**/
\*.pyc

If secrets are accidentally committed, rotate them immediately and purge them from Git history.

Use a private repository for projects with sensitive logic or configurations.

🤝 Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch (git checkout -b feature/YourFeature).
Commit your changes (git commit -m 'Add YourFeature').
Push to the branch (git push origin feature/YourFeature).
Open a Pull Request.

Please ensure your code follows the project’s coding style and includes appropriate tests.

👨‍💻 Author

Shan Naseem – Initial work
GitHub: @Shannaseem
