# 🤖 n8n Automation Workflows

> Free, production-ready n8n workflows built by a real AI automation freelancer.
> Steal them. Use them. Build on them.

[![Instagram](https://img.shields.io/badge/Instagram-@abdulrahmann.o-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/abdulrahmann.o)
[![GitHub stars](https://img.shields.io/github/stars/abduloid/n8n-automation-workflows?style=for-the-badge&color=yellow)](https://github.com/abduloid/n8n-automation-workflows/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## ⚡ What's Inside

| Workflow | What It Does | Stack |
|----------|-------------|-------|
| 🔗 [LinkedIn Auto Poster](#-linkedin-auto-poster) | Posts to LinkedIn daily — zero manual work | Google Sheets + Gemini + LinkedIn API |
| 📸 [Instagram Carousel Pipeline](#-instagram-carousel-pipeline) | Scrapes AI news → writes 10-slide carousel scripts automatically | RSS + Claude + n8n |

---

## 🔗 LinkedIn Auto Poster

**The problem:** Posting on LinkedIn consistently is painful. You forget. You run out of ideas. You get busy.

**The solution:** Add a topic. The system does the rest.

### How It Works
```
Google Sheets (topic added)
        ↓
Gemini 2.5 Pro writes post in your voice
        ↓
Auto posts to LinkedIn at your chosen time
        ↓
Marks row as "Posted" + saves content
        ↓
Sends you an email confirmation ✅
```

### Setup
1. Import `LinkedIn Auto Poster — Abdul Rahman.json` into n8n
2. Connect credentials:
   - ✅ Google Sheets OAuth
   - ✅ Google Gemini API
   - ✅ LinkedIn OAuth
   - ✅ SMTP Email
3. Create Google Sheet with these exact columns:

```
Topic | Status | Post Content | Date Posted
```

4. Add your topics with `Status = Pending`
5. Activate workflow — done.

### Customization
- Change posting time in the Schedule Trigger node
- Edit the prompt inside `Message a model` to match your voice
- Add more columns to track engagement

---

## 📸 Instagram Carousel Pipeline

**The problem:** Creating daily carousel content requires research, writing, and designing. It takes hours.

**The solution:** Wake up. Your carousel script is already written.

### How It Works
```
Daily trigger at 9AM PKT
        ↓
Scrapes RSS feeds (TechCrunch AI, Anthropic, OpenAI)
        ↓
Claude picks the most interesting story for your audience
        ↓
Claude writes a 10-slide carousel script in your voice
        ↓
Saves script to pending file for design builder
        ↓
🏁 Done — ready to design and post
```

### Slide Structure Claude Follows
- **Slide 1** — Hook that stops scrolling
- **Slides 2–8** — Content, insights, data
- **Slide 9** — Key takeaway
- **Slide 10** — CTA to follow

### Setup
1. Import `Instagram Carousel Pipeline — Abdul Rahman.json` into n8n
2. Connect credentials:
   - ✅ Anthropic API Key
3. Create your voice file at `/data/scripts/abdul-rahman-voice.txt`
4. Set your output path for pending carousels
5. Activate workflow — done.

### Voice File Example
```
You are writing Instagram carousel content for [Your Name].
Short, punchy sentences. Direct. No fluff.
Bold, practical, no-nonsense tone.
Never use: "In today's world", "Game-changer", "Leverage".
```

---

## 🛠 Requirements

- n8n (self-hosted or cloud)
- Google Sheets account
- Anthropic API key (Claude)
- Google Gemini API key
- LinkedIn Developer App
- SMTP email account

---

## 📁 Folder Structure

```
n8n-automation-workflows/
├── LinkedIn Auto Poster — Abdul Rahman.json
├── Instagram Carousel Pipeline — Abdul Rahman.json
└── README.md
```

---

## 🚀 More Workflows Coming

- [ ] Twitter/X Auto Poster
- [ ] Client Onboarding Pipeline
- [ ] PPE Detection Alert System
- [ ] Follow-up Sequence Automation
- [ ] Content Calendar Auto-Scheduler

**Star this repo to get notified when new workflows drop ⭐**

---

## 👤 About

Built by **Abdul Rahman** — AI Automation Freelancer from Pakistan 🇵🇰

I build automation systems for agencies and businesses that save 40+ hours a week.

- 🤖 10+ agents deployed
- ⏱ 40+ hours saved weekly for clients
- 🛠 Stack: n8n · Claude API · Python · Computer Vision

**Follow me on Instagram for daily AI automation content:**
[@abdulrahmann.o](https://instagram.com/abdulrahmann.o)

---

## ⭐ Support

If these workflows helped you — star the repo. It takes 1 second and means a lot.

And if you want a custom automation built for your business — DM me on Instagram.

---

*Built with 🤖 in Pakistan*
