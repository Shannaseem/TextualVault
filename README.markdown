# TextualVault

**TextualVault** is a Python-based application combining a **Textual User Interface (TUI)** with backend logic for data storage, email utilities, and user management. It uses **Python**, **SQLAlchemy** for database operations, and the `textual` TUI framework.

---

## 📂 Project Structure

```plaintext
TextualVault/
├── app/
│   ├── __init__.py       # Package initializer
│   ├── crud.py           # Create, Read, Update, Delete operations
│   ├── database.py       # Database connection and session management
│   ├── email_utils.py    # Functions for sending and handling emails
│   ├── main.py           # Main backend entry point
│   ├── models.py         # SQLAlchemy models for database tables
│   ├── tui_main.py       # Text-based User Interface entry point
├── .gitignore            # Git ignore rules
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
└── .env                  # Environment variables (ignored by Git)
```

> **Note**: The `.env` file contains sensitive information and is ignored by Git for security.

---

## 🚀 Features

- **Database Support**: SQLAlchemy ORM for efficient data storage and retrieval.
- **Email Utilities**: Send OTPs and notifications via configurable SMTP.
- **Textual UI**: Interactive command-line interface using the `textual` framework.
- **Modular Design**: Separate modules forContext: The user has been refining a `README.md` file for their `TextualVault` project, a Python-based application with a Textual User Interface (TUI), SQLAlchemy, and email utilities. They initially provided a `README.md` and requested updates to the folder structure, removal of the License section, and conversion to Markdown for proper GitHub rendering due to issues with the folder structure display. In the latest request, they asked for the "complete file of it," implying the final version of the `README.md` with all updates applied, ensuring it renders correctly on GitHub.

Action: I will provide the complete `README.md` file in clean Markdown, incorporating all requested changes:
- **Updated Folder Structure**: Using the user-provided structure with proper Markdown code block syntax (`plaintext`) to ensure correct rendering on GitHub.
- **Removed License Section**: As per the user's request to make the project "open for all."
- **GitHub-Friendly Formatting**: Using consistent headings, code blocks (`bash` for commands, `env` for `.env`, `plaintext` for structure), and clear spacing.
- **Previous Enhancements**: Retaining additions like the Contributing section, Prerequisites, and security notes from prior responses.
- **Corrected Syntax**: Ensuring `__init__.py` and other filenames render correctly without escaping underscores or bold formatting issues.

Since the user also asked for a `.gitignore` file previously, I’ll include a note on how to use it but won’t generate it again unless requested.

<xaiArtifact artifact_id="fc13a86c-953c-4541-9602-8564b7cb0108" artifact_version_id="8929810f-8261-4a17-9457-1e92c390bc63" title="README.md" contentType="text/markdown">

# TextualVault

**TextualVault** is a Python-based application combining a **Textual User Interface (TUI)** with backend logic for data storage, email utilities, and user management. It uses **Python**, **SQLAlchemy** for database operations, and the `textual` TUI framework.

---

## 📂 Project Structure

```plaintext
TextualVault/
├── app/
│   ├── __init__.py       # Package initializer
│   ├── crud.py           # Create, Read, Update, Delete operations
│   ├── database.py       # Database connection and session management
│   ├── email_utils.py    # Functions for sending and handling emails
│   ├── main.py           # Main backend entry point
│   ├── models.py         # SQLAlchemy models for database tables
│   ├── tui_main.py       # Text-based User Interface entry point
├── .gitignore            # Git ignore rules
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
└── .env                  # Environment variables (ignored by Git)
```

> **Note**: The `.env` file contains sensitive information and is ignored by Git for security.

---

## 🚀 Features

- **Database Support**: SQLAlchemy ORM for efficient data storage and retrieval.
- **Email Utilities**: Send OTPs and notifications via configurable SMTP.
- **Textual UI**: Interactive command-line interface using the `textual` framework.
- **Modular Design**: Separate modules for CRUD, models, and UI.
- **Environment Configuration**: Manage API keys, database credentials, and email settings via `.env`.

---

## 🛠 Installation

### Prerequisites
- Python 3.8 or higher
- PostgreSQL (for database support)
- A valid SMTP server account (e.g., Gmail, SendGrid)
- `git` for cloning the repository

### Steps
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Shannaseem/TextualVault.git
   cd TextualVault
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python -m venv .venv

   # Linux/Mac
   source .venv/bin/activate

   # Windows
   .venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   Create a `.env` file in the project root with:
   ```env
   DATABASE_URL=postgresql+psycopg2://user:password@localhost:5432/textualvault
   EMAIL_HOST=smtp.example.com
   EMAIL_PORT=587
   EMAIL_USER=your_email@example.com
   EMAIL_PASSWORD=your_email_app_password
   ```

---

## ▶ Usage

- **Run the backend**:
  ```bash
  python -m app.main
  ```

- **Run the TUI application**:
  ```bash
  python -m app.tui_main
  ```

---

## 🔐 Security Precautions

- **Never commit `.env`** to GitHub, as it contains sensitive credentials.
- Ensure `.gitignore` includes:
  ```plaintext
  .env
  .venv/
  __pycache__/
  *.pyc
  ```
- If secrets are accidentally committed, **rotate them immediately** and purge from Git history.
- Use a **private repository** for sensitive logic or configurations.

---

## 🤝 Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add YourFeature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/YourFeature
   ```
5. Open a Pull Request.

> Ensure your code follows the project’s coding style and includes tests.

---

## 👨‍💻 Author

- **Shan Naseem** – Initial work
- GitHub: [@Shannaseem](https://github.com/Shannaseem)