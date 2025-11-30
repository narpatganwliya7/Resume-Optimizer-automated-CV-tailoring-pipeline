# 🚀 Automated Resume Optimizer  
*A fully automated system that generates a job-specific optimized resume every morning.*

---

## 📌 Overview  

This project is an **end-to-end AI-powered automation** that tailors my resume to the latest job openings without any manual work.  
The system runs **daily at 8 AM**, pulls my original resume from Google Drive, scrapes new job listings from LinkedIn using Apify, analyzes job requirements using AI agents, and produces a new optimized resume aligned with each job.

The generated resume is saved back to Google Drive, and I receive a notification with the download link.

This workflow removes repetitive resume editing and transforms it into a fully automated pipeline.

---
## 🎬 Demo Video (GIF Preview)

![Demo GIF]([https://github.com/narpatganwliya7/Resume-Optimizer-automated-CV-tailoring-pipeline/blob/6135a43d53658babf34aa98b00263381d6b52f51/Media/IMG_2024.gif])


<p align="center">
  <img src="Media/IMG_2024.gif" alt="Automation Demo" width="800">
</p>




## ✨ Key Features  

### 🔄 Daily Automation  
Runs automatically every morning at **08:00 AM**.

### 📄 Resume Retrieval  
Fetches the latest version of my master resume from Google Drive.

### 🌐 Live Job Scraping (LinkedIn)  
Uses **Apify** to fetch fresh job postings—roles, descriptions, responsibilities, skills.

### 🧠 AI Job Matching Agent  
Analyzes:
- Job title  
- Required skills  
- Responsibilities  
- Experience level  

Then compares it with my resume.

### 🤖 AI Resume Builder Agent  
Generates a personalized, ATS-friendly resume including:
- Rewritten experience  
- Targeted achievements  
- Matched keywords  
- Clean formatting  

### 📄 Document Generator  
Creates a formatted Google Doc or PDF.

### ☁ Cloud Storage Export  
Uploads the final resume to Google Drive.

### 🔔 Optional Notifications  
Can notify via:
- Email  
- Telegram bot  

---

## 🧩 Tech Stack  

| Component | Technology |
|----------|------------|
| Automation Engine | n8n |
| AI Agents | OpenAI GPT-4.1 mini / GPT-4.1 |
| Web Scraping | Apify LinkedIn Job Scraper |
| Storage | Google Drive API |
| Notification | Gmail API + Telegram Bot |
| Document Creation | n8n Document Node |

---

## 🛠 Workflow Architecture  

1. **Scheduler Trigger** → Runs at 08:00 AM daily  
2. **Get Original Resume** → Fetch from Google Drive  
3. **Scrape LinkedIn Jobs** → Using Apify  
4. **Structured Output Parser** → Cleans job data  
5. **Job Matching Agent** → Compares job vs. resume  
6. **Resume Builder Agent** → Generates optimized resume  
7. **Limit/If Nodes** → Clean processing  
8. **Create Optimized Resume Document** → PDF/Doc  
9. **Upload to Google Drive**  
10. **Send Notification (Email/Telegram)**  

---

## 📸 Workflow Screenshot  
<p align="center">
  <img src="Media
/Screenshot 2025-11-30 103127.png" alt="Automation Demo" width="800">
</p>

