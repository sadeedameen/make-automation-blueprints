# Invoice Compliance Verification Automation

This project demonstrates an automated workflow for validating invoice compliance using AI and no-code tools. It is designed to reduce manual effort in finance operations by checking invoices, verifying calculations, and taking appropriate actions based on the results.

---

## Overview

The system monitors incoming emails for invoices, extracts the attached files, and uses an AI model to validate whether the invoice meets VAT compliance requirements. Based on the outcome, it either stores the invoice or notifies the sender about issues.

---

## Workflow

The automation is built as a sequence of steps:

1. **Monitor Emails**
   Watches for incoming emails with "invoice" in the subject and ensures an attachment is present.

2. **Extract Attachments**
   Retrieves the invoice file from the email for further processing.

3. **Upload to AI Model**
   Sends the invoice document to the AI system for analysis.

4. **Invoice Analysis**
   The AI checks:

   * Required invoice fields
   * VAT calculations
   * Total amounts
     It then returns a status: Pass or Fail, along with any identified issues.

5. **Decision Routing**
   The workflow branches based on the AI result:

   * If **Pass**: the invoice is stored in Google Drive
   * If **Fail**: a response email is sent requesting corrections

---

## Outcome

* Reduces manual invoice validation work
* Improves accuracy in compliance checks
* Speeds up communication with suppliers
* Creates a structured record of approved invoices

---

## Tech Stack

* Make
* Google Gemini AI
* Gmail
* Google Drive

---


## How to Use

1. Import the blueprint into Make
2. Connect your Gmail, Google Drive, and AI account
3. Configure the email filter and destination folder
4. Run the scenario

---

## Notes

This workflow is based on the module design outlined in the project documentation and can be extended for other tax systems or document validation use cases.

---

## Future Improvements

* Support for multiple tax systems (GST, EU VAT)
* Better reporting and tracking
* Additional notification channels

---

## License

This project is open for learning and experimentation.
