# n8n-automation-workflows
Free n8n automation workflows for freelancers and agency owners. Built by @abdulrahmann.o

# 🤖 n8n Automation Workflows

Free production-ready n8n workflows for freelancers and agency owners.
Built and battle-tested by [@abdulrahmann.o](https://instagram.com/abdulrahmann.o)

---

## 📦 Workflows

### 1. LinkedIn Auto Poster
Automatically generates and posts to LinkedIn daily — zero manual work.

**How it works:**
- You add a topic to Google Sheets
- Gemini AI writes the post in your voice
- Auto posts to LinkedIn at 11PM daily
- Marks row as Posted + saves content
- Sends you an email confirmation

**Stack:** n8n + Google Sheets + Gemini 2.5 Pro + LinkedIn API

---

## ⚙️ Setup

1. Import the JSON into your n8n instance
2. Connect your credentials:
   - Google Sheets OAuth
   - Google Gemini API
   - LinkedIn OAuth
   - SMTP Email
3. Create your Google Sheet with columns:
   `Topic | Status | Post Content | Date Posted`
4. Add topics with Status = `Pending`
5. Activate the workflow

---

## 🌐 Follow for More

New workflows dropped regularly.

- Instagram: [@abdulrahmann.o](https
