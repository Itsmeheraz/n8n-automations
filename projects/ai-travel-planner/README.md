# AI Travel Planner

An end-to-end AI travel research agent that turns a simple trip form into a complete, personalized roadmap — flights, hotels, budget, activities, and local food — delivered straight to your inbox.

🎥 [Watch on YouTube](https://www.youtube.com/@AutomateWithMeheraz)
🔗 [View on Portfolio](https://meherazhossain.com/#)

## Overview

Automates the entire travel-planning research process from form submission to a ready-to-read itinerary emailed directly to the traveler.

## Technical Logic & Workflow

1. **Simple Form Intake** — User submits origin, destination, dates, traveler count, email, and optional interests through a clean web form — no complicated inputs needed.
2. **Input Validation with Branching** — Every request is validated before processing; invalid submissions get a proper error response instead of silently failing or wasting API calls.
3. **Airport Code & Date Resolution** — A GPT-powered step resolves city names into correct airport codes and normalizes travel dates before any search runs, using a structured output schema for reliability.
4. **Live Multi-Source Research** — Simultaneously searches real flight prices, hotel options, and local activities & food recommendations through live travel APIs — not static, pre-written suggestions.
5. **Bad Resort Filtering** — Automatically filters out low-quality or irrelevant resort results before they ever reach the final itinerary.
6. **Flight Options with Comfort Details** — Surfaces multiple real flight options with pricing, duration, legroom, Wi-Fi, and even estimated carbon emissions for each.
7. **Curated Hotel Picks with Reasoning** — Each recommended hotel includes amenities, photos, and a written explanation of why it fits the traveler's style — couples, groups, road-trippers, etc.
8. **Personalized Activities & Local Food** — Matches beaches, hikes, and attractions to the user's stated interests, complete with local tips (best time to visit, crowd avoidance) and specific food recommendations.
9. **Automatic Budget Breakdown** — Compiles a clear cost overview covering flights, estimated resort range, and activity cost variability.
10. **AI Email Agent** — A dedicated email-writing agent assembles all researched data into a warm, well-structured HTML itinerary — trip summary, flights, resorts, budget, and activities — before sending.
11. **Instant Delivery** — The complete roadmap is emailed directly to the user's inbox as soon as processing finishes, with an immediate 'processing' response sent back to the form so the user isn't left waiting.
12. **Modular n8n Architecture** — Clean separation between trigger/validation, research/search, and AI email generation makes the workflow easy to extend with new destinations or data sources.

## Nodes / Tools Used

- Web form trigger (input intake)
- Validation/branching logic
- GPT (airport code + date resolution, structured output)
- Live travel APIs (flights, hotels, activities, food)
- Filtering logic (resort quality)
- AI email-writing agent
- Email/SMTP (delivery)

## Setup

1. Create the web form and connect it as the trigger
2. Add validation rules for required fields
3. Connect GPT credential for airport code/date resolution
4. Connect travel API credentials (flights, hotels, activities)
5. Connect email/SMTP credential for final delivery
