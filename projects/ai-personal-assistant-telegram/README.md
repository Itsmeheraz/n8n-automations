# AI Personal Assistant (Telegram-Based)

A self-hosted personal AI assistant that manages emails, meetings, and daily tasks through Telegram — with a morning briefing so your day starts with full clarity.

🎥 [Watch on YouTube](https://youtu.be/ium_fB8KcTQ?si=50wBgT02hmYzzHA)
🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Telegram-Native Control** — Runs entirely through Telegram — send a message like 'remind me to call this person tomorrow' and the assistant handles it.
2. **Allow-List Access** — Only listens to authorized senders, with a dedicated check to confirm the message is from the owner (boss) before acting.
3. **Voice Message Understanding** — Detects voice notes automatically, transcribes them via speech-to-text, and processes the request just like a typed message.
4. **Central AI Agent Core** — A single personal-assistant agent routes every request — task creation, event scheduling, email sending, and inbox checks — through one reasoning engine.
5. **Meeting & Task Management** — Can create calendar events, save daily tasks to a tracked list, and pull pending tasks or today's events on demand.
6. **Email Actions** — Sends emails and checks important incoming emails directly from a chat command — no need to open Gmail.
7. **Window Buffer Memory** — Maintains recent conversation context so follow-up requests stay coherent without repeating full instructions.
8. **Automated Morning Briefing** — On a daily schedule, it independently checks tasks, events, and important emails, then pushes a consolidated update straight to Telegram.
9. **Expandable Foundation** — Built on the same host, it's designed to extend into CRM automation, Google Sheets, WhatsApp follow-ups, website lead handling, and reporting.

## Nodes / Tools Used

- Telegram trigger (message + voice note intake)
- Allow-list/owner verification logic
- Speech-to-text (voice transcription)
- AI agent core (central request routing)
- Calendar (event creation + retrieval)
- Task tracking list
- Gmail (send + check important emails)
- Window buffer memory (conversation context)
- Schedule trigger (daily morning briefing)

## Setup

1. Create a Telegram bot and connect it as the trigger
2. Set up the allow-list with the authorized owner's Telegram ID
3. Connect speech-to-text credential for voice message transcription
4. Connect calendar and task-tracking credentials
5. Connect Gmail credential for sending and checking emails
6. Set the daily schedule time for the morning briefing
