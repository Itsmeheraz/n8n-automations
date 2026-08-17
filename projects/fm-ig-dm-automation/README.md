# AI Messenger & Instagram DM Automation

A dual-platform AI agent that manages Facebook Messenger and Instagram DMs together — tracking offline conversations, capturing leads, and seamlessly handing off to a human when needed.

[Watch in Action](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Dual-Platform Trigger** — A single Webhook and token captures incoming messages from both Messenger and Instagram simultaneously — no separate setup needed.
2. **Offline Message Tracking** — Even when the agent is offline, every conversation is tracked and stored in Supabase — so when the user returns, the AI already knows the full history.
3. **Smart Name Collection & Personal Greeting** — On the first message, the workflow collects the user's name and greets them personally, making every interaction feel human from the start.
4. **Emotional Intelligence & Human Handover** — Detects frustration or explicit requests for a human, then triggers a handover panel with 'I'll Handle This' or 'I'm Busy' — apologizing with a contact number if busy, or opening a full human-to-user chat if handled.
5. **10-Minute Auto-Resume** — If a human takes over and goes quiet for 10 minutes, the AI automatically steps back in — the conversation never stays stuck.
6. **Lead Capture with Telegram Summary** — Collected phone numbers sync instantly to Google Sheets, and a conversation summary is pushed to Telegram so the team knows exactly what was discussed.
7. **Voice Message Support** — Automatically transcribes and understands audio messages, then responds accordingly.
8. **RAG-Powered Knowledge Base** — Answers are grounded strictly in your provided data via retrieval-augmented generation — no hallucinations, no guesswork.
9. **Optional Image Reading** — Built-in support for reading and understanding user-sent images, ready to enable per use case.
10. **Fully Customizable Logic** — The entire architecture adapts to any business niche and can be tailored to any brand's exact workflow.

## Nodes / Tools Used

- Webhook (dual-platform trigger — Messenger + Instagram)
- Supabase (conversation storage + offline tracking)
- Name collection + personalized greeting logic
- Emotional intelligence / handover detection
- Human handover panel ('I'll Handle This' / 'I'm Busy')
- Auto-resume timer (10-minute inactivity trigger)
- Google Sheets (phone number/lead capture)
- Telegram (conversation summary delivery)
- Speech-to-text (voice message transcription)
- RAG knowledge base (retrieval-augmented generation)
- Image recognition (optional, per use case)

## Setup

1. Set up the Webhook and connect the token for both Messenger and Instagram
2. Connect Supabase credential for conversation and offline message storage
3. Configure the name-collection and greeting flow for first-time users
4. Set up the handover panel and connect the human agent's response options
5. Set the auto-resume timer duration (default 10 minutes)
6. Connect Google Sheets for lead/phone number capture
7. Connect Telegram credential for conversation summary delivery
8. Connect speech-to-text credential for voice message support
9. Connect the knowledge base source for RAG-grounded answers
10. Enable image reading if needed for your use case
