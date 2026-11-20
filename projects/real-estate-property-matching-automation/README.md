

# Real Estate Property Management & Buyer Matching Automation System

An end-to-end real estate automation system that collects property submissions through websites and Gmail, verifies property information, automatically organizes photos and videos in Google Drive, manages property approvals, and matches approved property listings with potential buyers based on their requirements — with daily matching and automated email notifications.

🎥 [Watch on YouTube](https://youtu.be/WGX2KbtXcIY)  🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Automated Website Property Submission** — Collects property details submitted by sellers through website forms using webhooks, including relevant information, property photos, and videos, without requiring manual data entry.

2. **Gmail Property Submission Processing** — Processes property information received through Gmail, allowing sellers to submit property details and attach supporting photos and videos directly through email.

3. **Automatic Data Verification** — Checks each property submission to determine whether all required information has been provided before proceeding with the next stage of the workflow.

4. **Automated Missing Information Requests** — Identifies incomplete property submissions and automatically sends an email requesting the missing details from the seller.

5. **Google Drive Folder Creation & File Organization** — Automatically creates a dedicated Google Drive folder using the seller's name and organizes their property photos and videos in that folder, whether submitted through the website or Gmail.

6. **Google Sheets Property Database** — Automatically records and updates submitted property information in Google Sheets, maintaining an organized database for property management, review, and approval.

7. **Automatic Owner Notifications** — Notifies the business owner about submitted property information, allowing the owner to review the details and determine whether the property should proceed to the next stage.

8. **Human-Controlled Property Approval** — Allows the business owner to manually review property submissions and approve or reject them based on the available information. Only approved properties proceed to buyer matching.

9. **Automated Seller Approval Confirmation** — Automatically sends an email to the property seller once their property has been approved by the owner, keeping the seller informed about the approval status.

10. **Daily Property Matching Automation** — Uses a scheduled workflow to check approved property listings against the requirements of potential buyers every day, identifying relevant properties without manually comparing each listing.

11. **Requirement-Based Buyer Matching** — Compares approved property information with buyers' submitted requirements, such as preferred location, property type, budget, and other available criteria, to identify potential matches.

12. **Automated Buyer Email Notifications** — Sends an automatic email to potential buyers when one or more approved properties match their requirements, allowing them to review relevant property listings.

13. **End-to-End Property Management Automation** — Connects website and Gmail submissions, missing information verification, Google Drive organization, Google Sheets updates, owner approval, seller notifications, and daily buyer matching into one centralized n8n workflow.

## Nodes / Tools Used

- **Webhook Trigger** — Collects property submissions from website forms.
- **Gmail Trigger** — Receives property details and attachments submitted through Gmail.
- **Data Extraction & Processing** — Extracts and structures property information received from different submission channels.
- **Data Validation Logic** — Checks submitted property information for missing required fields.
- **IF / Switch Nodes** — Handles conditional routing for complete and incomplete submissions, approval status, and matching results.
- **Gmail** — Sends missing information requests, seller approval confirmations, and buyer notifications.
- **Google Drive** — Creates seller-specific folders and stores submitted property photos and videos.
- **Google Sheets** — Stores property information, approval records, and data used in buyer matching.
- **Owner Notification Integration** — Sends submitted property information to the business owner for review.
- **Approval Status Logic** — Controls whether a property is eligible to proceed to buyer matching.
- **Schedule Trigger** — Runs daily property-to-buyer matching checks.
- **Property Matching Logic** — Compares approved property details with potential buyers' requirements.
- **n8n** — Orchestrates the complete automation workflow and connects the different services.

## Setup

1. Configure Website Property Submission.
2. Connect Gmail for Property Submissions.
3. Configure Property Data Verification.
4. Set Up Google Drive File Organization.
5. Create a Google Sheets Property Database.
6. Configure Owner Notifications & Approval.
7. Configure Seller Approval Emails.
8. Set Up Buyer Requirements Data.
9. Configure Daily Property-to-Buyer Matching.
10. Configure Automated Buyer Notifications.
