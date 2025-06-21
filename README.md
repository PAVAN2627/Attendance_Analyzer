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
