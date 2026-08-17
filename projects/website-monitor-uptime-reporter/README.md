# AI Website Monitor & Uptime Reporter

An autonomous monitoring agent that checks your websites around the clock, instantly alerts you on downtime, and sends a weekly AI-analyzed PDF report.

🎥 [Watch on YouTube](https://youtu.be/ium_fB8KcTQ?si=VTL3gt5pewFJgC26)
🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Multi-Site Check** — Automatically checks every website on your list on a recurring schedule, no manual monitoring needed.
2. **Status Detection** — Identifies whether a website is UP, DOWN, or running SLOW in real time.
3. **Deep Error Tracking** — Detects SSL, DNS, timeout, 404, 403, and 500+ server-level issues for precise diagnosis.
4. **Smart Delay Filter** — Waits before rechecking a flagged site to recheck before sending a down alert, avoiding false alarms from brief blips.
5. **Instant Alerts** — Sends immediate updates via Gmail and Telegram the moment a site stays down or shows issues.
6. **Temporary Downtime Tracker** — Still notifies you even if a site recovered on its own after a brief hosting hiccup or traffic spike — nothing slips by unnoticed.
7. **Google Sheets Database** — Maintains a complete history log and tracks the latest status of each site individually.
8. **Weekly AI Reports** — Generates a beautifully formatted PDF report — analyzed by AI, complete with suggested solutions — delivered straight to your inbox.
9. **Built to Protect Revenue** — Designed for website owners, digital agencies, SaaS founders, and businesses that can't afford to lose traffic, leads, or revenue to downtime.
10. **Modular n8n Architecture** — Separate branches for down/recovered states, recheck logic, and reporting make the system easy to extend or customize.

## Nodes / Tools Used

- Schedule trigger (recurring multi-site check)
- HTTP request / status check nodes
- Error detection logic (SSL, DNS, timeout, 4xx/5xx)
- Delay/recheck node (false-alarm filter)
- Gmail (alerts + weekly report delivery)
- Telegram (instant alerts)
- Google Sheets (history log + status database)
- AI report generation (PDF analysis)

## Setup

1. Add the list of websites to monitor in Google Sheets
2. Set the schedule trigger interval for checks
3. Connect Gmail and Telegram credentials for alerts
4. Configure the recheck delay to avoid false alarms
5. Connect AI credential for weekly report analysis and PDF generation
