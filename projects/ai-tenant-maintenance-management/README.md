# AI Tenant Maintenance Management

An AI-powered maintenance management workflow built for real estate and property management businesses. It handles tenant maintenance requests, issue classification, vendor assignment, SLA tracking, follow-ups, and reporting through a centralized automation system.

🔗 [View on Portfolio](https://meherazhossain.com/)

## Technical Logic & Workflow

1. **Maintenance Request Intake** — Receives maintenance requests through a webhook, processes the submitted information, generates a unique ticket ID, and records the request in Google Sheets.

2. **AI-Powered Issue Classification** — Uses GPT-4o to understand the maintenance issue, determine its urgency, and identify the appropriate vendor category. The AI response is converted into structured JSON for further processing.

3. **Automated SLA Calculation** — Calculates the resolution deadline based on the priority of each maintenance request:
   - Emergency — 3 hours
   - High — 24 hours
   - Normal — 72 hours
   - Low — 7 days

4. **Intelligent Vendor Assignment** — Matches maintenance requests with relevant vendors based on their service category and existing workload, with the option for human approval before assignment.

5. **Automated Communication** — Sends relevant updates to tenants, vendors, and property managers through Gmail and Telegram, reducing the need for manual follow-ups.

6. **SLA Monitoring & Escalation** — Regularly checks pending maintenance tickets, identifies overdue requests, and sends escalation notifications when resolution deadlines are exceeded.

7. **Tenant Confirmation & Ticket Reopening** — Once a vendor marks an issue as resolved, the tenant is asked to confirm whether the problem has been fixed. Based on the response, the ticket is either closed or reopened for further action.

8. **Automated Ticket Closure** — Includes a 48-hour auto-close mechanism for resolved tickets when no tenant response is received.

9. **Daily Maintenance Digest** — Generates a daily summary of maintenance requests for low and normal priority and notify to the management with suggested vendor.

10. **Weekly Performance Reporting** — Generates weekly reports to help property managers track maintenance activity, ticket status, and overall operational performance.

11. **Human-in-the-Loop Control** — Keeps property managers involved in important decisions while automating repetitive tasks, notifications, and ticket monitoring.

## Nodes / Tools Used

- n8n (workflow automation)
- Webhook triggers (maintenance request intake)
- OpenAI GPT-4o (issue classification and urgency assessment)
- Structured output parser (JSON-based AI responses)
- Google Sheets (ticket and vendor management)
- Gmail (tenant and vendor communication)
- Telegram (management alerts and notifications)
- Code nodes (ticket IDs, SLA calculation, and business logic)
- IF and Switch nodes (conditional routing)
- Schedule triggers (SLA monitoring and automated reporting)
- REST APIs and webhooks (system communication)

## Setup

1. Import the workflow into your n8n instance
2. Connect your OpenAI API credential
3. Create a Google Sheets document with separate TICKETS and VENDORS sheets
4. Configure the required ticket and vendor data fields
5. Connect Gmail credentials for automated communication
6. Create a Telegram bot and configure management notifications
7. Configure the maintenance request and response webhooks
8. Set up vendor categories, workload limits, and assignment rules
9. Configure SLA deadlines and escalation conditions
10. Set the schedule for ticket monitoring, daily digests, and weekly reports
11. Test ticket creation, vendor assignment, resolution, tenant confirmation, and escalation before activating the workflow


