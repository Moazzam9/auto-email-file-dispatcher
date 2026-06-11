# 📧 Auto Email File Dispatcher

![Automation Banner](https://media.giphy.com/media/26ufdipQqU2lhNA4g/giphy.gif)

A powerful **bulk email automation system** that sends personalized emails with automatically matched file attachments based on CSV data and file naming patterns.

---

## 🚀 Features

- 📩 Send bulk personalized emails
- 📎 Auto-attach files (PDF, DOCX, images, etc.)
- 🧠 Smart matching using **ID or Name**
- 📊 Auto-generated delivery report
- ⏱ Random delay system to avoid spam detection
- 🔄 Works for ANY use case (not limited to internships)

---

## 🖼️ Workflow Preview

![Workflow](https://media.giphy.com/media/l0HlQ7LRalRkZ6sLy/giphy.gif)


CSV Data + ZIP Files → Matching Engine → Email Sender → Report Generated


---

## 📂 Project Structure


auto-email-file-dispatcher/
│── auto_email_sender.py
│── report.csv (generated)
│── files/ (extracted attachments)


---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/auto-email-file-dispatcher.git
cd auto-email-file-dispatcher
2. Install dependencies
pip install pandas
📄 CSV Format

Your CSV file must contain:

Full Name	Email Address	ID
John Doe	john@email.com	1234
📦 File Naming Format (Important)

Your ZIP files should be named like:

John_Doe_1234.pdf
Invoice_5678.pdf
Certificate_91011.pdf

The system automatically matches:

ID → Highest priority match
Name → Fallback match
▶️ How to Run
python auto_email_sender.py

Then enter:

CSV file path
ZIP file path

The system will:

Extract files
Match recipients
Send emails
Generate report
📊 Output Report

After execution:

report.csv

Contains:

Sent emails
Missing attachments
Failed deliveries
🔐 Security Warning

⚠️ NEVER upload your Gmail password to GitHub

Use Gmail App Password instead:

👉 https://support.google.com/accounts/answer/185833

Replace in code:

APP_PASSWORD = "YOUR_APP_PASSWORD_HERE"
⏱ Anti-Spam Protection

To avoid email blocking:

Random delay between emails (5–10 sec)
Sequential sending
SMTP secure connection
🧠 Use Cases
HR offer letters
Invoice distribution
Certificate delivery
School/college results
Business document automation
Notification systems
📈 Tech Stack
Python 🐍
Pandas 📊
SMTP Email System 📧
ZIP File Processing 📦
Regex Smart Matching 🧠
🎯 Future Improvements
🌐 Web dashboard (React + Flask)
📡 API-based email sending
📊 Real-time tracking UI
☁️ Cloud deployment version
🔐 OAuth Gmail login (no password needed)
👨‍💻 Author

Moazzam KK
Full Stack Developer

⭐ If you like this project

Give it a ⭐ on GitHub and share it!


---
