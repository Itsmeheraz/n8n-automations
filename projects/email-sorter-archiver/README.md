# AI Email Sorter & Archiver

An autonomous AI agent that reads, understands, and organizes your Gmail inbox in real-time — auto-archiving spam and promotions while surfacing what actually matters.

🎥 [Watch on YouTube](https://www.youtube.com/@AutomateWithMeheraz)
🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Real-Time Gmail Watcher** — Instantly detects every new incoming email the moment it lands in the inbox.
2. **Context-Aware Reading** — Powered by a GPT reasoning engine that actually reads and understands email content — not just keyword or sender-based filtering.
3. **Smart Priority Detection** — Automatically identifies what's important — client messages, bank alerts, invoices, meeting requests — and keeps it visible in the inbox.
4. **Silent Auto-Archiving** — Newsletters, promotions, and no-reply spam are quietly archived before they ever clutter the inbox.
5. **Dynamic Label Management** — Fetches existing Gmail labels first, and only creates a new one if nothing relevant exists — keeping the labeling system clean and non-redundant.
6. **Context Memory** — Retains short-term memory across runs so the agent stays consistent in how it classifies similar emails over time.
7. **Full Content Retrieval** — Pulls the complete email body (not just subject lines) before making a sorting decision, for higher classification accuracy.
8. **Sync Delay Buffer** — Built-in delay node ensures Gmail's API has fully synced the new message before the agent processes it, preventing missed reads.
9. **Zero Manual Rules** — No static filters or keyword rules to maintain — the agent adapts naturally to how real emails are actually written.
10. **Modular n8n Architecture** — Success/Error branches are separated for reliability, making the workflow easy to extend with alerts, logging, or CRM sync.
11. **Time-Saving at Scale** — Turns a ~20-minute daily manual sorting chore into a fully autonomous background process.

## Nodes / Tools Used

- Gmail trigger (real-time watcher)
- GPT reasoning engine (context-aware classification)
- Gmail labels API (dynamic label fetch/create)
- Memory node (context retention across runs)
- Delay node (sync buffer)
- Success/Error branching logic

## Setup

1. Connect Gmail credential and enable the real-time trigger
2. Connect GPT credential for context-aware reading and classification
3. Configure the delay node duration to match Gmail API sync time
4. Review/adjust priority categories (client, bank, invoice, meeting, etc.)
5. Set up Success/Error branches for logging or alerts as needed
