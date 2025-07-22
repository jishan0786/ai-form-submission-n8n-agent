# ai-form-submission-n8n-agent
Automates form submissions, stores ratings in Airtable, and uses Gemini AI to evaluate and update records.


# Form Submission AI Agent (n8n)

This workflow automates the review process for form submissions using Google Gemini AI. It:
- Captures form data
- Stores records in Airtable
- Switches logic based on role (video editor or designer or AI manager)
- Uses Gemini AI to generate review summaries
- Updates Airtable with final output

## 🛠 Tech Stack
- n8n
- Google Gemini Pro
- Airtable
- AI logic using custom prompts

## ⚙️ Workflow Overview

![Workflow Screenshot](./screenshots/workflow.png)

## 🚀 Setup Instructions
1. Clone this repo
2. Import the JSON workflow into your n8n instance
3. Configure the following:
   - Airtable credentials
   - Gemini API key
   - Webhook trigger for form submissions
4. Run & test

## 📦 Example Output
```json
{
  "Name": "Jane Doe",
  "Role": "Graphic Designer",
  "AI Review": "Jane has a sharp eye for modern design aesthetics..."
}
