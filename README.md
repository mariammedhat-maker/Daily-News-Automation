# 📰 AI News Automation Bot

An automated AI-powered workflow that collects the latest news from an RSS feed, summarizes the news using Google Gemini, and sends the results directly to Telegram.

## 🚀 Project Overview

This project is an **automated news delivery system** built with **n8n**.

The workflow runs automatically every day at **11:30 AM**, retrieves news from an RSS feed, selects the top **5 news articles**, uses **Google Gemini** to process and summarize the content, and then sends the results directly to a **Telegram bot**.

The goal is to automate the process of collecting, processing, and delivering relevant news without any manual intervention.

## ⚙️ Workflow

The automation follows these steps:

1. ⏰ **Schedule Trigger**
   - Runs automatically every day at **11:30 AM**.

2. 📰 **RSS Read**
   - Retrieves the latest news articles from the configured RSS feed.

3. 🔢 **Limit**
   - Selects the top **5 news items**.

4. 🤖 **Google Gemini**
   - Processes the news using Google Gemini.
   - Generates a concise and readable summary for each article.

5. 📩 **Telegram**
   - Sends the processed news directly to a Telegram chat.

### Workflow Architecture

```text
Schedule Trigger
       ↓
    RSS Read
       ↓
      Limit
    (5 Items)
       ↓
 Google Gemini
       ↓
 Send Telegram Message
