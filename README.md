# Automated Motivational Email Sender (n8n Workflow)

##  Project Overview

This project is an automation workflow built using **n8n** that sends personalized motivational emails to users whose tasks are due today. The workflow reads user data from a Google Sheet, filters records based on the due date, and sends a customized email to each user using Gmail.

This project demonstrates practical skills in workflow automation, data filtering, personalization, and real-world integration of cloud services.

---

##  Objective

To automatically send a lovely and motivational message to each user whose due date matches today's date — without manual effort.

---

##  Key Features

*  Reads data from Google Sheets
*  Filters rows where **Due Date = Today**
*  Personalizes email using each user's name
*  Sends emails automatically via Gmail
*  Processes multiple users at once
*  No coding required (low-code automation)

---

##  Workflow Architecture

**Google Sheets → Filter → Set Node → Gmail Node → Emails Sent**

### Step-by-step Flow:

1. **Google Sheets Node** — Fetches all records from the sheet
2. **Filter Node** — Selects only rows where due date equals today's date
3. **Set Node** — Prepares personalized fields (Name, Email, Message)
4. **Gmail Node** — Sends customized email to each user

---

## Input Data Format (Google Sheet)

| Name   | Email                                     | Due Date   |
| ------ | ----------------------------------------- | ---------- |
| User A | [usera@email.com](mailto:usera@email.com) | 2026-02-25 |
| User B | [userb@email.com](mailto:userb@email.com) | 2026-02-25 |

---

##  Email Content (Example)

Subject: A Little Boost for Today 

Hi {{Name}},

Just a gentle reminder that today is a wonderful opportunity to move one step closer to your goals 

Believe in yourself, stay positive, and remember that every small effort counts. You’ve got this 

Wishing you a productive and beautiful day ahead 

Warm regards,
Automation Bot

---

##  Tools & Technologies Used

* n8n (Workflow Automation)
* Google Sheets API
* Gmail API

---

##  How to Run the Project

1. Create a Google Sheet with Name, Email, and Due Date columns
2. Connect Google Sheets to n8n
3. Configure Filter node to match today's date
4. Customize email template
5. Execute workflow

---

##  Learning Outcomes

* Real-world automation design
* Data filtering and transformation
* Personalized communication at scale
* Integration of multiple services

---

##  Future Improvements

* Schedule automation to run daily
* Add WhatsApp/Telegram notifications
* Dashboard for tracking sent emails
* AI-generated personalized messages

