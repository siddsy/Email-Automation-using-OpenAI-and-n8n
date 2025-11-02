# Email-Automation-using-OpenAI-and-n8n
An n8n automation that fetches your Gmail emails, summarises them using OpenAI, and sends a clean daily summary report.
# 📧 Automated Email Summary Workflow

This workflow automatically fetches your Gmail emails from a chosen time range (e.g., past 24 hours), summarizes them using **OpenAI**, and sends a neat HTML summary to your inbox.  
---

## 🌟 Overview

| 🔹 Step | Description |
|:--|:--|
| **Trigger** | Starts manually or on a schedule (via Cron). |
| **Fetch Emails** | Pulls emails from Gmail using Google Cloud API. |
| **Organize Data** | Extracts sender, recipient, CC, and mail body. |
| **Summarize Emails** | Uses OpenAI to generate a readable summary. |
| **Send Report** | Sends the summary to your chosen email addresses. |

---

## 🧩 Workflow Preview

Here’s what the workflow looks like in n8n:

![Workflow Screenshot](./160f5ff0-089d-442c-874e-90151e65cde2.png)

---

## ⚙️ Setup Guide

### 1. Create Gmail API Credentials (GCP)

1. Go to [Google Cloud Console](https://console.cloud.google.com/).
2. Create a **new project** (or select an existing one).
3. Navigate to **APIs & Services → + ENABLE APIS AND SERVICES**.
4. Search for **Gmail API** and enable it.
5. Go to **Credentials → Create Credentials → OAuth client ID**.
6. Choose **Web application**, and add your n8n instance redirect URI:  
