# 🌐 TalentSphere Elevate

**AI-Powered Career Guidance Platform** — built with **Python, Streamlit, SQLite, Pandas, NumPy, Plotly, Scikit-learn, and ReportLab**.

TalentSphere Elevate guides **High School Students, College Students, and Working Professionals** through their entire career journey — from self-discovery and skill-building to resumes, interviews, certifications, internships, and professional growth.

The platform also includes a dedicated **Admin Portal** for managing users, courses, career paths, learning materials, quizzes, analytics, notifications, and reports.

---

## ✨ Highlights

* 🔐 **Full Authentication**

  * Signup
  * Login
  * Forgot Password
  * Logout
  * No email verification required

* 🎯 **Automatic Dashboard Redirection**

  * Users are automatically redirected to a category-specific dashboard after signup.

* 🧑‍🎓 **High School Dashboard**

  * 10 career-development modules
  * Extended profile including:

    * School
    * Board
    * Study year
    * City
    * Favorite subjects
    * Career interest area
    * Target exam
  * Personalized course recommendations
  * Profile-based learning recommendations
  * Quiz result matching

* 🎓 **College Dashboard**

  * 12 career-development modules
  * Extended profile including:

    * College
    * Branch
    * Specialization
    * CGPA
    * Graduation year
    * GitHub
    * LinkedIn
    * Portfolio
    * Target role
  * ATS Resume Checker
  * GitHub Portfolio Review
  * LinkedIn Profile Review
  * Internship recommendations
  * Hackathon recommendations
  * Live navigation to career platforms

* 💼 **Working Professional Dashboard**

  * 9 professional-development modules
  * Extended profile including:

    * Company
    * Designation
    * Industry
    * Years of experience
    * Current CTC
    * Work location
    * LinkedIn
    * Key skills
    * Career goal
  * Salary Benchmark
  * Networking & Visibility Builder
  * AI-predicted certifications
  * Industry trend analysis
  * Trending-role navigation
  * Job-board navigation

* 🛡️ **Admin Portal**

  * Manage Users
  * Manage Courses
  * Manage Career Paths
  * Upload Materials
  * Create Quizzes
  * View Analytics
  * Send Notifications
  * Generate Reports

* 🤖 **AI-Powered Features**

  * Rule-based AI
  * Scikit-learn
  * TF-IDF
  * Cosine Similarity
  * Career recommendations
  * Resume/ATS scoring
  * Skill analysis
  * Mock interview feedback
  * Chatbot
  * Certification recommendations
  * Optional OpenAI integration
  * Optional Gemini integration

* 📄 **PDF Generation**

  * PDF certificates
  * PDF reports
  * Profile Verification Reports
  * Unique verification codes
  * Assessment history
  * Quiz history
  * Learning progress
  * Goal history
  * Certificate history

* 📎 **Document Upload & Analysis**

  * Resume PDF/DOCX/TXT analysis
  * GitHub profile PDF analysis
  * LinkedIn profile PDF analysis
  * Resume update assistance

* 🔗 **Live Career Platform Navigation**

  * Internshala
  * LinkedIn Jobs
  * Naukri
  * Indeed
  * Devpost
  * Unstop
  * HackerEarth
  * MLH
  * Glassdoor
  * Meetup
  * Eventbrite

* 📊 **Interactive Dashboards**

  * Donut charts
  * Line charts
  * Bar charts
  * Radar charts
  * Gauge charts
  * Plotly visualizations

* 🎨 **Premium UI**

  * Glassmorphism
  * Gradient hero banners
  * Smooth animations
  * Responsive layout
  * Modern dashboard components

---

# 🆕 What's New

| Area                                | Update                                                                                                                                                              |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **High School Profile**             | Added school name, board, study year, city, favorite subjects, career interest area, and target exam. Courses and quiz results are ranked against these selections. |
| **College Profile**                 | Added college name, branch, specialization, CGPA, graduation year, GitHub, LinkedIn, portfolio, and target role.                                                    |
| **ATS Resume Checker**              | Now accepts PDF, DOCX, and TXT file uploads instead of manually pasted resume text.                                                                                 |
| **Internship Recommendations**      | Added live searches on Internshala, LinkedIn, Indeed, and Naukri with a free-text search option.                                                                    |
| **Hackathon Updates**               | Added live searches on Devpost, Unstop, HackerEarth, and MLH with a free-text search option.                                                                        |
| **GitHub Portfolio Review**         | Analyzes an uploaded PDF export of the user's GitHub profile.                                                                                                       |
| **LinkedIn Profile Review**         | Analyzes an uploaded PDF export of the user's LinkedIn profile and recommends personal-branding courses.                                                            |
| **PDF Reports**                     | Added `generate_verification_report()` for generating detailed profile verification reports.                                                                        |
| **Professional Profile**            | Added company, designation, industry, experience, CTC, work location, LinkedIn, skills, and career goal.                                                            |
| **Industry Trend Dashboard**        | Displays trending job roles by industry with live job-search navigation.                                                                                            |
| **Certification Suggestions**       | Expanded certification suggestions to 7 domains and added AI-predicted certifications based on entered skills.                                                      |
| **Resume Update Assistant**         | Accepts a resume file and target role and identifies present and missing role-specific keywords.                                                                    |
| **Salary Benchmark**                | Compares current CTC against market ranges by role and experience.                                                                                                  |
| **Networking & Visibility Builder** | Provides a weekly networking checklist and links to LinkedIn Events, Meetup, and Eventbrite.                                                                        |

---

# 🗂️ Project Structure

```text
TalentSphere_Elevate/
│
├── app.py
├── requirements.txt
│
├── .streamlit/
│   └── config.toml
│
├── assets/
│   └── style.css
│
├── database/
│   ├── db.py
│   └── talentsphere.db
│
├── auth/
│   └── auth_utils.py
│
├── utils/
│   ├── ai_engine.py
│   ├── pdf_generator.py
│   ├── charts.py
│   └── ui.py
│
└── modules/
    ├── common.py
    ├── high_school.py
    ├── college.py
    ├── professional.py
    └── admin.py
```

---

# 📁 Project Components

| File / Folder             | Description                                                              |
| ------------------------- | ------------------------------------------------------------------------ |
| `app.py`                  | Main application entry point and router                                  |
| `requirements.txt`        | Python dependencies                                                      |
| `.streamlit/config.toml`  | Streamlit theme configuration                                            |
| `assets/style.css`        | Glassmorphism UI, animations, and styling                                |
| `database/db.py`          | SQLite database, schema, CRUD operations, and seed data                  |
| `auth/auth_utils.py`      | Signup, login, logout, and password management                           |
| `utils/ai_engine.py`      | AI engine with rule-based and optional LLM integration                   |
| `utils/pdf_generator.py`  | PDF certificates and reports                                             |
| `utils/charts.py`         | Reusable Plotly chart components                                         |
| `utils/ui.py`             | Reusable UI components                                                   |
| `modules/common.py`       | Common profile, notification, chatbot, progress, and certificate modules |
| `modules/high_school.py`  | High School dashboard modules                                            |
| `modules/college.py`      | College dashboard modules                                                |
| `modules/professional.py` | Working Professional dashboard modules                                   |
| `modules/admin.py`        | Admin Portal modules                                                     |

---

# 🚀 Getting Started

## Prerequisites

Make sure the following are installed:

* Python 3.10+
* pip
* Git
* VS Code

---

## 1. Open the Project

Open the `TalentSphere_Elevate` folder in VS Code.

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
python3 -m venv venv
```

Activate it:

```bash
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Run the Application

```bash
streamlit run app.py
```

The application will normally open at:

```text
http://localhost:8501
```

---

# 🔐 Default Admin Login

The database and default administrator account are created automatically during the first application launch.

```text
Username: admin
Password: Admin@123
```

> **Security:** Change the default administrator password before deploying the application to production.

---

# 🤖 AI Engine

TalentSphere Elevate works out of the box without requiring an external AI API key.

The default offline AI engine uses:

* Scikit-learn
* TF-IDF
* Cosine Similarity
* Rule-based logic
* Keyword matching
* Profile-based scoring

These techniques power features such as:

* Career recommendations
* Resume/ATS scoring
* Skill analysis
* Career-path matching
* Mock interview feedback
* Certification recommendations
* Chatbot responses

This means the application remains fully functional without external API configuration.

---

# 🔌 Optional Live AI

TalentSphere Elevate can optionally use **OpenAI or Gemini**.

No application code changes are required.

## OpenAI

### Windows CMD

```cmd
set OPENAI_API_KEY=your_api_key
```

### Windows PowerShell

```powershell
$env:OPENAI_API_KEY="your_api_key"
```

### macOS/Linux

```bash
export OPENAI_API_KEY="your_api_key"
```

## Gemini

### Windows CMD

```cmd
set GEMINI_API_KEY=your_api_key
```

### Windows PowerShell

```powershell
$env:GEMINI_API_KEY="your_api_key"
```

### macOS/Linux

```bash
export GEMINI_API_KEY="your_api_key"
```

Then run:

```bash
streamlit run app.py
```

The `utils/ai_engine.py` module detects the configured API key and routes AI requests through the appropriate provider.

> **Never commit API keys to GitHub.**

---

# 🗄️ Database

TalentSphere Elevate uses **SQLite** as its local database.

The database is automatically initialized using `init_db()` when the application starts.

## Database Tables

```text
users
admins
assessments
learning_progress
courses
career_paths
notifications
certificates
reports
resume_data
quiz_results
mock_interview_results
coding_practice
projects
achievements
goals
chat_history
admin_actions
```

The `users` table includes a `profile_extra` JSON column for category-specific information such as:

* School details
* College details
* Professional details
* Career preferences
* Skills
* Social profiles

Database migrations are automatically applied during startup so existing databases can be upgraded safely.

---

# 🔄 Reset the Database

To reset all local application data, delete:

```text
database/talentsphere.db
```

Then restart the application:

```bash
streamlit run app.py
```

The database will be recreated automatically with the default seed data.

---

# 🧭 User Journey

```text
Sign Up / Login
       │
       ▼
Select Career Category
       │
       ├───────────────┬────────────────┐
       ▼               ▼                ▼
 High School        College       Professional
       │               │                │
       └───────────────┼────────────────┘
                       ▼
                Complete Profile
                       │
                       ▼
                Assessments & Quizzes
                       │
                       ▼
                  AI Analysis
                       │
                       ▼
           Personalized Recommendations
                       │
                       ▼
              Learning & Skill Building
                       │
                       ▼
            Career & Resume Tools
                       │
                       ▼
       Internships / Jobs / Hackathons
                       │
                       ▼
             Progress & Certificates
```

### Detailed User Journey

1. User signs up without email verification.
2. User is redirected to the appropriate category dashboard.
3. User completes their profile.
4. User explores assessments and quizzes.
5. AI analyzes strengths, weaknesses, interests, and skills.
6. Personalized recommendations are generated.
7. User completes learning activities.
8. Progress is tracked through visual dashboards.
9. Users can analyze resumes and professional profiles.
10. Users can explore internships, jobs, hackathons, and certifications.
11. Certificates and reports can be generated as PDFs.
12. Administrators manage the platform through the Admin Portal.

---

# 🧑‍🎓 High School Dashboard

The High School dashboard helps students understand their interests, strengths, and possible career directions.

## Profile

* School name
* Board
* Study year
* City
* Favorite subjects
* Career interest area
* Target exam

## Features

* Career assessments
* Personalized courses
* Career-path recommendations
* Learning dashboard
* Quizzes
* Progress tracking
* Goals
* Certificates
* Notifications
* AI recommendations

---

# 🎓 College Dashboard

The College dashboard focuses on employability, internships, projects, technical skills, and professional branding.

## Profile

* College name
* Branch
* Specialization
* CGPA
* Graduation year
* GitHub
* LinkedIn
* Portfolio
* Target role

## Features

* ATS Resume Checker
* Resume Update Assistant
* GitHub Portfolio Review
* LinkedIn Profile Review
* Internship recommendations
* Hackathon recommendations
* Coding practice
* Projects
* Certifications
* Mock interviews
* Career paths
* Skill development
* Live opportunity navigation

---

# 💼 Working Professional Dashboard

The Working Professional dashboard helps users improve career growth, market positioning, professional visibility, and skills.

## Profile

* Company
* Designation
* Industry
* Years of experience
* Current CTC
* Work location
* LinkedIn
* Key skills
* Career goal

## Features

* Salary Benchmark
* Industry Trends
* Trending Job Roles
* AI-predicted Certifications
* Certification recommendations
* Networking & Visibility Builder
* Career planning
* Skill analysis
* Resume tools
* Job-search navigation
* Professional development tracking

---

# 🛡️ Admin Portal

The Admin Portal provides centralized management of the TalentSphere Elevate platform.

## Admin Features

* 👥 Manage Users
* 📚 Manage Courses
* 🧭 Manage Career Paths
* 📂 Upload Materials
* 📝 Create Quizzes
* 📊 View Analytics
* 🔔 Send Notifications
* 📄 Generate Reports
* ⚙️ Manage Platform Data
* 📋 Track Admin Actions

---

# 📄 PDF Features

ReportLab is used to generate downloadable PDF documents.

## Generated Documents

* Certificates
* Assessment reports
* Career reports
* Profile reports
* Profile Verification Reports

## Profile Verification Report

The verification report can contain:

* Profile snapshot
* Assessment history
* Quiz history
* Learning progress
* Goals
* Certificates
* Unique verification code

---

# 📎 Document Analysis

TalentSphere Elevate supports document-based career analysis.

## Supported Formats

```text
PDF
DOCX
TXT
```

## Supported Documents

* Resume
* GitHub profile PDF
* LinkedIn profile PDF

This reduces manual data entry and allows the platform to extract useful career information from uploaded documents.

---

# 🔗 Career & Opportunity Platforms

TalentSphere Elevate provides live navigation to external career platforms.

## Internships & Jobs

* Internshala
* LinkedIn Jobs
* Naukri
* Indeed
* Glassdoor

## Hackathons & Competitions

* Devpost
* Unstop
* HackerEarth
* MLH

## Networking

* LinkedIn Events
* Meetup
* Eventbrite

---

# 📊 Visualization

The platform uses Plotly and other visualization libraries for interactive dashboards.

## Charts

* 🍩 Donut charts
* 📈 Line charts
* 📊 Bar charts
* 🕸️ Radar charts
* 🎯 Gauge charts

These visualizations are used for:

* Learning progress
* Skill analysis
* Assessment results
* Career readiness
* Performance tracking
* Salary benchmarking
* Analytics

---

# 🛠️ Tech Stack

| Layer                | Technology                                  |
| -------------------- | ------------------------------------------- |
| Programming Language | Python                                      |
| UI Framework         | Streamlit                                   |
| Database             | SQLite                                      |
| Data Processing      | Pandas, NumPy                               |
| Visualization        | Plotly, Matplotlib                          |
| AI / ML              | Scikit-learn                                |
| AI Techniques        | TF-IDF, Cosine Similarity, Rule-Based Logic |
| Optional AI APIs     | OpenAI, Gemini                              |
| PDF Generation       | ReportLab                                   |
| Styling              | Custom CSS                                  |
| Version Control      | Git & GitHub                                |

---

# 🏗️ Architecture

```text
┌──────────────────────────────────────────────┐
│                  Streamlit UI                │
├──────────────────────────────────────────────┤
│              Application Router              │
│                   app.py                     │
├──────────────────────────────────────────────┤
│              Dashboard Modules               │
│ High School │ College │ Professional │ Admin │
├──────────────────────────────────────────────┤
│                Common Modules                │
│ Profile │ Progress │ Chatbot │ Certificates  │
├──────────────────────────────────────────────┤
│                   AI Engine                  │
│ TF-IDF │ Similarity │ Rules │ OpenAI/Gemini │
├──────────────────────────────────────────────┤
│                 Utility Layer                │
│ Charts │ PDF Generator │ UI Components       │
├──────────────────────────────────────────────┤
│                    SQLite                   │
│                  Database                    │
└──────────────────────────────────────────────┘
```

---

# 🔐 Security Notes

The project uses local password hashing with **HMAC-SHA256**.

For production deployment, it is recommended to:

* Use HTTPS.
* Change the default administrator password.
* Store API keys using secure environment variables or secrets management.
* Never commit API keys to GitHub.
* Add `.env` files to `.gitignore`.
* Exclude local databases from public repositories.
* Use a managed authentication solution where appropriate.
* Use a production-grade database for large-scale deployments.
* Restrict administrative access.

---

# 📌 Recommended `.gitignore`

```gitignore
# Virtual environment
venv/
.venv/
env/

# Python cache
__pycache__/
*.py[cod]

# Environment variables
.env
.env.*

# Streamlit secrets
.streamlit/secrets.toml

# Local SQLite database
*.db
*.sqlite
*.sqlite3

# IDE
.vscode/
.idea/

# Operating system
.DS_Store
Thumbs.db

# Logs
*.log
```

> **Important:** Never commit passwords, API keys, `.env` files, or sensitive database files to a public repository.

---

# 📦 Installation Summary

```bash
# Clone repository
git clone https://github.com/YOUR_USERNAME/talentsphereelevate_teamc.git

# Enter project
cd talentsphereelevate_teamc

# Create virtual environment
python -m venv venv

# Activate on Windows
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run application
streamlit run app.py
```

---

# 🧪 Development

Run the application using:

```bash
streamlit run app.py
```

To use a custom port:

```bash
streamlit run app.py --server.port 8501
```

---

# 🚀 Future Enhancements

Potential future improvements include:

* 🌍 Multi-language career guidance
* ☁️ Cloud database support
* 📱 Progressive Web App support
* 🔔 Advanced notification system
* 🧠 Advanced ML recommendation models
* 📊 Career-readiness scoring
* 🎤 Voice-based career assistant
* 🤝 Mentor-student matching
* 💬 Advanced AI career chatbot
* 📈 Labor-market analytics
* 🔗 Additional job and internship integrations
* 🏢 Enterprise career-development features
* 📱 Dedicated mobile application

---

# 🤝 Contributing

Contributions are welcome.

## Contribution Steps

1. Fork the repository.
2. Create a feature branch.

```bash
git checkout -b feature/your-feature
```

3. Make your changes.
4. Test the application.
5. Commit your changes.

```bash
git add .
git commit -m "Add your feature"
```

6. Push your branch.

```bash
git push origin feature/your-feature
```

7. Open a Pull Request.

---

# 📜 License

This project is licensed under the **MIT License**.

See the [`LICENSE`](LICENSE) file for the complete license text.

---

# 👨‍💻 Team

## TalentSphere Elevate — Team C

Built with ❤️ for learners, students, job seekers, and working professionals.

---

# ⭐ Support the Project

If you find **TalentSphere Elevate** useful, consider giving the repository a ⭐ on GitHub.

---

**TalentSphere Elevate — Empowering career decisions with AI, data, and personalized guidance.**
