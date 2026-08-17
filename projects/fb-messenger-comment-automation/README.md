# AI Facebook Messenger & Comment Automation

An autonomous Facebook Messenger AI agent that holds natural, human-like conversations with customers — answering product questions, sending images, checking stock, taking orders, and following up — while also replying to post comments and converting interested commenters into private inbox conversations.

[Watch in Action](https://meherazhossain.com/#)

## Overview

Automates the full customer journey on Facebook — starting with real Messenger conversations (product Q&A, image-based lookups, stock checks, order taking, follow-ups) and extending to public post comments, converting engaged commenters into private sales conversations. The owner stays notified on every order and error in real time.

## Technical Logic & Workflow

1. **Human-Like Messenger Conversations** — Handles real customer chats in Messenger — answering questions, discussing products, and following up naturally, just like a human sales rep would.
2. **Product Image Handling** — Sends product images when asked, and can also receive an image from the user, identify the product in it, and reply with matching details.
3. **Stock Verification** — Checks live stock availability before confirming a product to the customer, avoiding orders for out-of-stock items.
4. **Order Creation & Update** — Takes new orders directly through the conversation and updates them as details are confirmed, keeping order records current.
5. **Owner Order Notifications** — Instantly notifies the business owner whenever a new order is placed or updated.
6. **Post-Aware Comment Understanding** — Before replying to a comment, the agent reads and understands the specific post it belongs to, so its reply stays relevant to that post's content.
7. **Automatic Comment Reply** — Responds to comments on posts automatically, keeping engagement active without manual moderation.
8. **Bad Comment Detection & Owner Approval** — Flags negative, abusive, or spam comments, notifies the owner before taking any action, and only deletes the comment once the owner confirms 'Yes.'
9. **Comment-to-Inbox Conversion** — Identifies commenters showing genuine interest and automatically opens a private Messenger conversation with them to continue the sales flow.
10. **Day/Night Availability Mode** — Can be configured to stay inactive during the day and only respond at night (or vice versa), based on business hours.
11. **Persistent Cross-Session Memory** — Remembers what was discussed with a user earlier in the day, so if that same user messages again at night, the AI recalls the earlier conversation instead of starting fresh.
12. **Voice Message Support** — Automatically transcribes and understands audio messages, then responds accordingly.
13. **Built-In Error Handling** — Every node is monitored; if any step fails, the owner is notified immediately so nothing silently breaks.
14. **Offline Message Tracking** — Even when the agent is offline, every conversation is tracked and stored in Supabase — so when the user returns, the AI already knows the full history.
15. **Emotional Intelligence & Human Handover** — Detects frustration or explicit requests for a human, then triggers a handover panel with 'I'll Handle This' or 'I'm Busy' — apologizing with a contact number if busy, or opening a full human-to-user chat if handled.
16. **10-Minute Auto-Resume** — If a human takes over and goes quiet for 10 minutes, the AI automatically steps back in — the conversation never stays stuck.
17. **Lead Capture with Telegram Summary** — Collected phone numbers sync instantly to Google Sheets, and a conversation summary is pushed to Telegram so the team knows exactly what was discussed.
18. **RAG-Powered Knowledge Base** — Answers are grounded strictly in your provided data via retrieval-augmented generation — no hallucinations, no guesswork.

## Nodes / Tools Used

- Facebook Messenger trigger (DM intake)
- Facebook comment trigger (post comment intake)
- AI agent core (conversation handling, product Q&A, order flow)
- Image recognition (product identification from user images)
- Stock/inventory check
- Order creation/update logic
- Owner notification (order + error alerts)
- Comment understanding + reply generation
- Comment-to-Messenger handoff logic
- Day/Night schedule control
- Persistent memory/database (cross-session conversation history)
- Speech-to-text (voice message transcription)
- Error-handling branches (per-node monitoring)
- Supabase (offline conversation tracking)
- Human handover panel ('I'll Handle This' / 'I'm Busy')
- Auto-resume timer (10-minute inactivity trigger)
- Google Sheets (order capture)
- Telegram (conversation summary delivery when asked for human)
- RAG knowledge base (retrieval-augmented generation)

## Setup

1. Connect Facebook Page credential for both Messenger and comment triggers
2. Connect the AI credential for conversation handling and comment reply generation
3. Connect the product database/stock source for inventory checks
4. Connect the order system (sheet/database) for order creation and updates
5. Set the owner's notification channel (Telegram/Email) for orders and errors
6. Configure day/night active hours
7. Connect the memory/database store for persistent conversation history
8. Connect speech-to-text credential for voice message support
9. Connect Supabase credential for offline conversation storage
10. Set up the handover panel and connect the human agent's response options
11. Set the auto-resume timer duration (default 10 minutes)
12. Connect Google Sheets for lead/phone number capture
13. Connect Telegram credential for conversation summary delivery
14. Connect the knowledge base source for RAG-grounded answers
