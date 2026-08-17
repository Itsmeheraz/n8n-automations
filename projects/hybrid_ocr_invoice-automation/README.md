# Hybrid OCR Invoice Automation

An intelligent invoice processing agent that detects duplicate files, handles both searchable and scanned PDFs, extracts structured data with AI, and keeps your invoice database updated automatically.

🎥 [Watch on YouTube](https://www.youtube.com/@AutomateWithMeheraz)
🔗 [View on Portfolio](https://meherazhossain.com/#)

## Technical Logic & Workflow

1. **Google Drive Trigger** — Automatically activates the moment a new invoice file is uploaded — no manual downloading needed.
2. **Duplicate Prevention** — Checks the File ID against Google Sheets before processing, ensuring the same invoice is never processed twice.
3. **Smart Format Detection** — Automatically determines whether an invoice is a searchable PDF or a scanned/image-based PDF before choosing an extraction method.
4. **Dual Extraction Pipeline** — Uses direct text extraction for searchable PDFs, and falls back to Mistral OCR for scanned or image-based invoices — covering both formats reliably.
5. **Binary Fallback Handling** — If initial text extraction fails, the workflow automatically retrieves the binary file and re-attempts extraction through the OCR path.
6. **Merged Data Stream** — Combines outputs from both the direct-extraction and OCR branches into a single unified data path before AI processing.
7. **AI-Powered Information Extraction** — An OpenAI-driven agent reads the merged text and pulls out structured invoice details — vendor, amount, date, and line items.
8. **Auto Database Update** — Extracted invoice data is automatically appended to Google Sheets, keeping your invoice records always current.
9. **Internal Team Notification** — Sends an email to the internal team with the extracted summary and a direct link to the original PDF.

## Nodes / Tools Used

- Google Drive (trigger + file storage)
- Google Sheets (duplicate check + database)
- PDF text extraction (searchable PDFs)
- Mistral OCR (scanned/image-based PDFs)
- OpenAI (structured data extraction)
- Email/SMTP (internal notification)

## Setup

1. Connect Google Drive credential and set the folder trigger
2. Connect Google Sheets credential for duplicate checking and database storage
3. Connect Mistral OCR credential for scanned invoice fallback
4. Connect OpenAI credential for structured extraction
5. Connect email credential for internal team notifications
