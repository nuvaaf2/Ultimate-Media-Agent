<div align="center">

# 🎬 Ultimate Media Agent

### Multi-Platform AI Media Agent — Controlled Entirely via Telegram

[![n8n](https://img.shields.io/badge/Built%20with-n8n-FF6D00?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://telegram.org)
[![Google Drive](https://img.shields.io/badge/Google%20Drive-API-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)](https://drive.google.com)

> ⚠️ **Status: Demo / Prototype** — Core workflows built and tested. Not yet in production deployment.

*One Telegram bot to rule them all — search Instagram, TikTok & Google Docs, edit images, manage your calendar, label emails, and handle contacts. All through natural language.*

</div>

---

## 📌 Overview

Ultimate Media Agent is a multi-platform AI assistant controlled entirely through a single **Telegram bot**. Instead of jumping between apps, users send natural language commands to the bot, which routes them to the right automation: searching social media content, managing Google Drive documents, editing images, scheduling calendar events, labeling Gmail, and more — all powered by **GPT-4.1-mini** for smart intent understanding.

---

## ✨ Features

- 🔍 **Multi-Platform Content Search** — Search and retrieve content across Instagram, TikTok, and Google Docs from one bot
- 🧠 **AI-Powered Query Understanding** — GPT-4.1-mini interprets natural language commands and routes them correctly
- 🖼️ **Image Editing** — Send an image to the bot and apply edits via text commands
- 📅 **Calendar Event Management** — Create, update, and query Google Calendar events through chat
- 📧 **Email Labeling** — Automatically label and organize Gmail using AI
- 👤 **Contact Agent** — Look up and manage contacts via natural language
- 🗂️ **Google Drive Integration** — Search, retrieve, and summarize documents on demand

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation & agent routing |
| **OpenAI GPT-4.1-mini** | Natural language understanding & AI responses |
| **Telegram Bot API** | Primary user interface |
| **Google Drive API** | Document search & retrieval |
| **Gmail API** | Email labeling & management |
| **Google Calendar API** | Event creation & management |

---

## 🔄 How It Works

```
User sends a natural language message to Telegram Bot
        ↓
GPT-4.1-mini classifies intent
        ↓
n8n routes to the correct sub-workflow:
   ├── Content Search  →  Instagram / TikTok / Google Docs
   ├── Image Edit      →  Image processing workflow
   ├── Calendar        →  Google Calendar API
   ├── Email           →  Gmail label/search workflow
   └── Contacts        →  Contact lookup workflow
        ↓
Result returned to user via Telegram
```

---

## 🚀 How to Use

### Prerequisites
- [n8n](https://n8n.io) (self-hosted or cloud)
- OpenAI API key
- Telegram Bot Token (via [@BotFather](https://t.me/botfather))
- Google Cloud project with Drive, Gmail & Calendar APIs enabled

### Setup Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/nuvaaf2/ultimate-media-agent.git
   cd ultimate-media-agent
   ```

2. **Import the workflow**
   - Open your n8n instance
   - Go to **Workflows → Import from file**
   - Select `ultimate-media-agent-workflow.json`

3. **Configure credentials**
   - Add your **OpenAI API key**
   - Add your **Telegram Bot Token**
   - Connect **Google OAuth** (Drive + Gmail + Calendar scopes)

4. **Activate the workflow**
   - Toggle to **Active**
   - Message your bot and try a command like:
     > *"Find my latest TikTok ideas doc on Google Drive"*
     > *"Schedule a meeting tomorrow at 3pm"*
     > *"Label all emails from John as Important"*

---

## 💬 Example Commands

| Command | Action |
|---------|--------|
| `"Search TikTok for trending cooking videos"` | Fetches content results |
| `"Find my Q3 report on Google Drive"` | Searches and returns Drive doc |
| `"Add a meeting with Sarah on Friday at 2pm"` | Creates calendar event |
| `"Label all promo emails as Marketing"` | Applies Gmail label |
| `"Edit this image — remove the background"` | Triggers image edit workflow |

---

## 📂 Repository Structure

```
ultimate-media-agent/
├── ultimate-media-agent-workflow.json   # n8n workflow export
```

---

## 📸 Workflow Preview

> <img width="1196" height="640" alt="image" src="https://github.com/user-attachments/assets/9d9c4f16-1e4c-429c-b653-6785078c2a9a" />


---

## 🔮 Roadmap

- [ ] Deploy to production (24/7 uptime)
- [ ] Add WhatsApp interface support
- [ ] Expand to YouTube & LinkedIn content search
- [ ] Add voice message command support
- [ ] User-specific memory & personalization

---

## 👤 Author

**Nuvaaf A N** — AI Automation Engineer | n8n Builder

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/nuvaaf-a-n-0b53a5341/)
[![GitHub](https://img.shields.io/badge/GitHub-nuvaaf2-181717?style=flat&logo=github)](https://github.com/nuvaaf2)

---

<div align="center">
⭐ Star this repo if you'd like to see it go live!
</div>
