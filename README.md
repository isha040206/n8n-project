# 🎉 Birthday Email Automation Workflow using n8n

An automated birthday email workflow built with **n8n** that checks employee birthdays from **Google Sheets** every day and automatically sends personalized birthday wishes with a beautiful greeting card image via **Gmail**.

---

## 📌 Project Overview

This workflow eliminates the manual process of remembering and sending birthday wishes.

Every day at the scheduled time, the workflow:

- Reads employee data from Google Sheets.
- Compares each employee's birth date with today's date.
- Identifies employees celebrating their birthday.
- Generates a personalized birthday message.
- Downloads a birthday greeting card image.
- Sends an email with the greeting card attached using Gmail.

---

## 🚀 Features

- ⏰ Automatic daily scheduling
- 📄 Reads employee data from Google Sheets
- 🎂 Birthday date verification
- 📧 Personalized birthday emails
- 🖼️ Birthday greeting card attachment
- 👤 Employee photo support
- 🔄 Fully automated workflow
- 📎 Gmail integration
- ⚡ No manual intervention required

---

## 🛠️ Technologies Used

- n8n
- Google Sheets
- Gmail API
- HTTP Request Node
- JavaScript (Code Node)
- Schedule Trigger
- Merge Node
- IF Node

---

## 📂 Workflow

```
Schedule Trigger
        │
        ▼
Google Sheets
        │
        ▼
Loop Over Employees
        │
        ▼
Check Birthday (IF)
        │
   Birthday Today?
      │      │
     Yes     No
      │       │
      ▼       └── Next Employee
Generate Message
      │
      ▼
Download Greeting Card
      │
      ▼
Download Employee Photo
      │
      ▼
Merge Files
      │
      ▼
Rename Attachments
      │
      ▼
Send Gmail
```

---

## 📋 Google Sheet Format

| Name | Email id | Birthdate | Photo |
|------|----------|-----------|-------|
| John Doe | john@gmail.com | 15/07 | Image URL |

---

## 📧 Email Sent

**Subject**

```
Happy Birthday <Employee Name> 🎉
```

**Message**

```
Dear <Employee Name>,

Wishing you a very Happy Birthday 🎂🎉

Have a wonderful year ahead filled with happiness,
success, and good health.

Best Regards,
Team
```

---

## ⚙️ Workflow Nodes

| Node | Purpose |
|------|----------|
| Schedule Trigger | Runs automatically every day |
| Google Sheets | Reads employee records |
| Loop Over Items | Processes each employee |
| IF | Checks today's birthday |
| Set | Creates personalized message |
| HTTP Request | Downloads birthday card |
| HTTP Request | Downloads employee photo |
| Merge | Combines image files |
| Code | Renames attachments |
| Gmail | Sends birthday email |

---

## 📁 Requirements

- n8n
- Google Account
- Gmail OAuth Credentials
- Google Sheets OAuth Credentials

---

## ▶️ Setup

1. Install n8n.
2. Import the workflow JSON.
3. Connect your Gmail account.
4. Connect your Google Sheets account.
5. Update the Google Sheet with employee information.
6. Activate the workflow.

The workflow will automatically send birthday emails every day.

---

## 📸 Sample Workflow

```
Google Sheets
      ↓
Loop
      ↓
Birthday Check
      ↓
Generate Message
      ↓
Download Images
      ↓
Merge
      ↓
Send Gmail
```

---

## 🎯 Use Cases

- Companies
- HR Teams
- Schools
- Colleges
- Organizations
- Small Businesses

---

## 🔮 Future Enhancements

- HTML birthday templates
- Company logo support
- WhatsApp birthday messages
- Microsoft Outlook integration
- Slack notifications
- Teams notifications
- PDF birthday certificates
- Dynamic AI-generated greeting cards

---

## 👩‍💻 Author

**Isha Prajapati**

B.Tech – Agricultural Information Technology (AIT)

- GitHub: https://github.com/isha040206
- LinkedIn: www.linkedin.com/in/isha-prajapati0402

---

## ⭐ If you found this project helpful, don't forget to Star the repository.
