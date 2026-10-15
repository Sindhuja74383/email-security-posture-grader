# 🟣 NGP-053 – Email Security Posture Grader

## 📌 Project Overview
An AI-assisted email security assessment workflow developed using n8n. It retrieves SPF and DMARC DNS TXT records, evaluates email authentication policies, assigns security grades, and sends reports through Telegram.

## 🎯 Objectives
- Retrieve DNS TXT records using Google DNS-over-HTTPS.
- Analyze SPF and DMARC email authentication policies.
- Grade email security posture from A to F.
- Explain identified security concerns.
- Send reports through Telegram.
- Log assessment results in an n8n Data Table.

## 🛠️ Technologies Used
- n8n Cloud
- Google DNS-over-HTTPS API
- SPF and DMARC
- AI Agent with Google Gemini
- Telegram Bot
- n8n Data Tables
- JavaScript

## ⚙️ Workflow
1. Start the workflow manually.
2. Prepare DNS queries for the selected domains.
3. Retrieve TXT records through Google's DNS API.
4. Parse SPF and DMARC records.
5. Use an AI Agent to assess the security posture.
6. Format the assessment report.
7. Store the results in a Data Table.
8. Send the report through Telegram.

## 🔍 Test Domains
- `apache.org`
- `example.com`

## 📊 Expected Output
The workflow produces a report containing:
- Domain name
- SPF record
- DMARC record and policy
- Security grade
- Severity
- Reasons for the assessment
- Execution ID and IST timestamp

## 🔐 Security Considerations
- Configure credentials separately in n8n.
- Never publish API keys, bot tokens, or passwords.
- Review exported workflow JSON before sharing.
- Validate AI-generated assessments against the underlying DNS records.

## 🚀 Setup
1. Download the workflow JSON from this repository.
2. Import it into an n8n instance.
3. Configure the required AI and Telegram credentials.
4. Configure the required chat ID variable and Data Table.
5. Test the workflow and verify the generated report.

## 👩‍💻 Author
Sindhuja C M

Cybersecurity | Email Security | Workflow Automation
