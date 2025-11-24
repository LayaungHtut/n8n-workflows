# 🔧 Setup Instructions

## 1. Import the Workflow
In **n8n**:

- Go to **Workflows → Import**
- Upload: `workflows/telegram-ai-assistant.json`

## 2. Add Required Credentials
In **n8n**, configure:

- **Telegram Bot API**
- **Google Gemini API** (PaLM / Generative Language API)

> ⚠️ *No credentials are stored in this repo.*

---

# ⚙️ How It Works

## 🖼️ Image Messages
- Detects if a Telegram message contains a **photo**
- Downloads the image  
- Sends it to the **Main Image Analysis Agent**
- Gemini AI analyzes:
  - Image description  
  - Objects  
  - Text  
  - Scenes  
  - Characters  
- Output is processed through a **Markdown-safe formatter**
- Sends clean, readable results back to Telegram

## ✍️ Text Messages
- Routes plain text to the **Secondary Chat Agent**
- Provides **natural, friendly conversation**
- Supports **English + Burmese**
- Maintains context via a **memory buffer**
- Output is sanitized to avoid **MarkdownV2 errors**

---

# 🔐 Security Notes
- No secrets or API keys are included in this repository  
- `.gitignore` prevents uploading sensitive files  
- Workflow JSON contains **no embedded credentials**  
- All secure data must be added via **n8n Credentials Manager**

---

# 📬 Contact
If you need help, improvements, or customizations, feel free to open an issue or reach out anytime.
