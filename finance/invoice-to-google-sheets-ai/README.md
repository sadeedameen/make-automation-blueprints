# Invoice Data Extraction to Google Sheets (AI Automation)

## Overview

This automation reads invoice emails from Gmail, extracts key invoice details using AI (Gemini), and stores the structured data in Google Sheets.

It eliminates manual data entry and helps maintain a clean and searchable invoice database.

---

## Data Extracted

* Invoice Number
* Invoice Date
* Vendor Name
* Total Amount
* Tax Amount
* Currency
* Due Date

---

## How to Import the Blueprint

1. Download the `blueprint.json` file
2. Log in to your Make account
3. Create a new scenario
4. Click the three-dot menu → **Import Blueprint**
5. Upload the file
6. The scenario will be created automatically

---

## Required Connections

After importing, reconnect the following services:

* Gmail
* Gemini AI
* Google Sheets

Make sure to update:

* Gmail account connection
* Gemini API connection
* Google Spreadsheet
* Sheet name

---

## Module Flow

### 1. Gmail – Watch Emails

Monitors incoming emails with:

* Subject containing "invoice"
* Attachments

### 2. Gmail – List Attachments

Retrieves invoice attachments from the email.

### 3. Gemini AI – Upload File

Uploads the invoice file for processing.

### 4. Gemini AI – Extract Data

Extracts structured invoice data in JSON format.

### 5. Google Sheets – Add Row

Stores extracted data as a new row in Google Sheets.

---

## Result

Whenever a new invoice email arrives, the system automatically extracts the data and stores it in Google Sheets without manual intervention.

---

## Notes

* Ensure your Gmail filters match your invoice format
* AI accuracy may vary depending on invoice design
* You can extend this workflow with alerts or validations

---

## File

* `blueprint.json` — Make automation blueprint

---

## Use Cases

* Accounting automation
* Expense tracking
* Finance team workflows
* Small business operations

---
