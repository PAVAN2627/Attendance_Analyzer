# 📊 Attendance Analyzer Agent (n8n Workflow)

An AI-powered, fully autonomous attendance analyzer that:
- 🕒 Analyzes daily attendance data (CSV)
- ✅ Determines who is Present, Late, or Absent
- 📄 Generates a color-coded HTML attendance report
- 📤 Sends the report automatically via email
- 🔁 Runs daily without human interaction

---

## 🚀 Features

| Feature                        | Description                                        |
|-------------------------------|----------------------------------------------------|
| ⏱️ Autonomous Execution         | Scheduled using n8n's Schedule Trigger             |
| 📥 CSV Input                   | CSV fetched from GitHub (daily file)               |
| 📊 Status Classification       | Function node assigns Present / Late / Absent     |
| 📄 Report Generation           | Generates HTML report with color-coded table      |
| 📧 Auto Email Delivery         | Sends the report via email (no manual step)        |
| 🧠 (Optional) AI Remarks       | Prepared for integration with OpenAI for insights  |

---

## 🧱 Workflow Structure

```plaintext
Schedule Trigger
    ↓
HTTP Request (CSV from GitHub)
    ↓
Function Node: Parse CSV
    ↓
Function Node: Classify Status
    ↓
Function Node: Generate HTML Report
    ↓
Email Node: Send Report


## Scnreeshot


![Screenshot 2025-06-22 000247](https://github.com/user-attachments/assets/f7688f09-7f0e-413b-bdf3-5a1ea5a6c488)



![OP 1](https://github.com/user-attachments/assets/89ddfe1b-b344-49a2-961b-1ca354d86d44)



![op2](https://github.com/user-attachments/assets/4111b12a-3dd3-4400-9e76-7e6f2bd80dcb)

