# n8n-subscription-tracker
An automated subscription management system built with n8n, Google Sheets, and Google Gemini, featuring expiration tracking and email notifications.
# 📅 Automated Subscription Tracker

An automated **subscription management and tracking system** built with n8n. It helps manage client subscriptions, calculate expiration dates, monitor remaining days, and send automatic email notifications before and when subscriptions expire.

## 🚀 Project Overview

This workflow automates subscription management using a form connected to Google Sheets.

When a new subscription is submitted, the system processes its duration, calculates the expiration date, and stores the client's information. It then monitors subscriptions automatically and sends email reminders based on their expiration status.

## ⚙️ Workflow Architecture

The project consists of two main automation processes:

### 1. Subscription Registration

1. **Form Trigger** – Collects client information, project details, subscription date, duration, and email.
2. **Google Gemini AI** – Converts the subscription duration into a number of days.
3. **JavaScript** – Calculates the subscription expiration date.
4. **Google Sheets** – Stores or updates subscription records using the Client ID.

### 2. Subscription Monitoring

1. **Schedule Trigger** – Starts the monitoring process automatically.
2. **Google Sheets** – Retrieves registered subscriptions.
3. **Loop Over Items** – Processes subscriptions individually.
4. **JavaScript** – Updates the remaining subscription days.
5. **IF Conditions** – Checks whether a subscription has 3 days remaining or has expired.
6. **Gmail** – Sends automatic email notifications to clients.

## 🛠️ Technologies Used

- **n8n** – Workflow automation.
- **Google Gemini** – AI-powered duration processing.
- **Google Sheets** – Subscription database.
- **JavaScript** – Date calculations and data processing.
- **Gmail** – Automated email notifications.

## ✨ Key Features

- Automated subscription registration.
- AI-powered duration conversion.
- Automatic expiration date calculation.
- Daily subscription monitoring.
- Automatic email reminders 3 days before expiration.
- Expiration notifications.
- Client and project information management.

## 📋 Requirements

- An n8n instance.
- Google Gemini API credentials.
- Google Sheets account.
- Gmail account.
- A configured Google Sheets document.

## 🔧 Setup

1. Download the workflow JSON file from this repository.
2. Import it into your n8n instance.
3. Configure Google Gemini credentials.
4. Connect your Google Sheets account and select your spreadsheet.
5. Configure Gmail credentials.
6. Set the Schedule Trigger to run daily.
7. Test the registration and notification processes before activating the workflow.

## 🎯 Project Goals

- Simplify subscription management.
- Reduce manual tracking.
- Prevent missed subscription deadlines.
- Improve client communication through automated notifications.

## 👨‍💻 Author

**Mouadh Hadid**

AI Automation Developer | n8n | Python | JavaScript

---

*Developed as part of my portfolio in workflow automation and intelligent business solutions.*
