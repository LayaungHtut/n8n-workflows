# 📚 n8n Timetable Assistant Workflow

This repository contains an n8n workflow that powers a Telegram-based timetable assistant.  
It uses Google Sheets, Gemini AI, and n8n’s automation engine to answer questions about class schedules and find available rooms.

---

## 🚀 Features

- AI-powered timetable assistant (Gemini)
- Fetches data from Google Sheets
- Telegram bot interface
- Smart sheet selection
- Free-room detection logic
- Memory buffer for better conversations

---

## 🔧 Setup Instructions

### 1. Import the Workflow  
In n8n:
- Go to **Workflows → Import**
- Upload: `workflows/timetable-assistant.json`

### 2. Add Required Credentials

In n8n, configure:

- **Telegram API**
- **Google Sheets OAuth2**
- **Google Gemini API**

(No credentials are stored in this repo.)

---

## 🔐 Security Notes

- No secrets are included in this repository.  
- `.gitignore` prevents accidental uploads of env/credentials files.  
- Workflow JSON contains no `credentials` blocks or webhook secrets.

---

## 📬 Contact

Feel free to open an issue or reach out if you need help.


