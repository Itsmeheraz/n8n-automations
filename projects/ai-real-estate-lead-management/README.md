# AI Real Estate Lead Management & Automation System

An intelligent AI-powered automation system that captures, qualifies, and scores real estate leads, answers client inquiries using RAG and conversation memory, books appointments through Gmail, and manages automated follow-ups — all through a centralized CRM workflow.

🎥 [Watch on YouTube](https://youtu.be/5M-9U7J4UwY?si=NYOZqgGXQeOA8dh3) 🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Automated Website Lead Capture** — Collects incoming real estate leads through website webhooks, automatically processing customer information without manual data entry.
2. **Smart Duplicate Detection** — Checks incoming information against existing records, identifies duplicate leads, and updates existing data instead of creating redundant entries.
3. **AI Lead Scoring** — Analyzes each lead, assigns a score from 1–100, and automatically classifies prospects as Hot, Warm, or Cold for better sales prioritization.
4. **Google Sheets CRM** — Automatically updates lead information, qualification scores, categories, contact details, and current status in a centralized database.
5. **AI Data Verification & Replies** — Checks whether all required information is available. Sends a confirmation email for complete leads or automatically requests missing details from incomplete leads.
6. **Supabase Conversation Memory** — Stores lead information and conversation history, allowing the AI agent to remember previous interactions and maintain context across client conversations.
7. **Intelligent Gmail Inquiry Handling** — Automatically processes incoming emails from clients who want to learn about available properties, ask questions about the company, or request an appointment.
8. **RAG-Powered Client Support** — Uses a connected RAG knowledge base to answer property-related and company-related questions with relevant information and context-aware responses.
9. **Instant Owner Notifications** — Automatically notifies the business owner when lead information is confirmed, keeping the owner informed while the system handles client communication.
10. **AI Appointment Booking** — Handles meeting requests received through Gmail, checks calendar availability, and books appointments when the requested slot is available. Otherwise, suggests three alternative date/time slots and notifies both the client and owner after successful booking.
11. **Intelligent Follow-Up Automation** — Runs daily checks on Warm and Cold leads and automatically sends follow-up emails at different scheduled intervals based on their qualification category.
12. **Smart Follow-Up Control** — Checks each lead's latest status before sending emails and automatically stops follow-ups when a client replies or reaches the maximum limit of five follow-ups, allowing the owner to take over.
13. **End-to-End Lead Lifecycle Management** — Connects lead capture, AI qualification, CRM updates, contextual email conversations, appointment booking, and automated follow-ups into one system that helps real estate businesses manage leads more efficiently.

## Nodes / Tools Used

- Webhook Trigger (website lead capture)
- Duplicate detection & data validation logic
- AI Agent / LLM (lead scoring, qualification & communication)
- Conditional routing (Hot / Warm / Cold)
- Google Sheets (CRM database & lead tracking)
- Supabase (persistent conversation memory)
- Gmail Trigger (property inquiries, company questions & appointment requests)
- RAG Knowledge Base (property & company information)
- Gmail (confirmations, automated replies & follow-ups)
- Owner notification integration
- Google Calendar (availability checking & appointment booking)
- Schedule Trigger (daily follow-up automation)
- Follow-up status & limit checking
- n8n (workflow orchestration)

## Setup

1. Connect the website webhook to automatically collect incoming real estate leads.
2. Create a Google Sheets CRM database to store lead details, qualification scores, status, and follow-up information.
3. Configure duplicate detection and data validation logic.
4. Connect an AI model and configure lead scoring from 1–100 with Hot, Warm, and Cold classifications.
5. Set up Supabase to maintain lead information and conversation memory.
6. Connect a RAG knowledge base containing property details and company information.
7. Configure Gmail to handle incoming property inquiries, company-related questions, appointment requests, and automated email responses.
8. Set up owner notifications and connect Google Calendar for meeting availability checks and appointment scheduling.
9. Configure daily follow-up schedules for Warm and Cold leads, including reply detection and a maximum five-follow-up limit.
10. Test the complete workflow with website leads, duplicate submissions, missing information, Gmail inquiries, appointment requests, and follow-up scenarios.
