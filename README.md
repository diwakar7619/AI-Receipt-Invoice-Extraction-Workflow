# README  — AI Receipt & Invoice Extraction Workflow

# AI Receipt & Invoice Extraction Workflow

Author: Pratham Diwakar

## Overview

An AI-powered expense automation workflow built using n8n that automatically processes receipts and invoices from Google Drive.

The system performs OCR extraction, AI-based structured data extraction, expense categorization, Google Sheets logging, automated file organization, and intelligent file renaming.

This workflow supports both image and PDF invoices.

---

## Features

- Automated Google Drive monitoring
- OCR text extraction for PDFs and images
- AI-powered structured information extraction
- Automatic expense categorization
- Google Sheets database logging
- Processed/Error folder routing
- Dynamic file renaming
- Multi-format support (PDF, PNG, JPG)
- End-to-end workflow automation

---

## Tech Stack

- n8n
- OpenAI GPT Models
- Google Vision OCR API
- Google Drive API
- Google Sheets API

---

## Workflow Architecture

1. Google Drive monitors the `Unprocessed` folder
2. Files are downloaded automatically
3. Files are converted to Base64
4. Workflow detects file type
5. OCR extracts raw text
6. OpenAI extracts structured expense data
7. Data is logged into Google Sheets
8. Files are moved to Processed/Error folders
9. Files are renamed dynamically

---

## Screenshots

### Main Workflow

![Workflow](images/workflow-overview.png)

### Example Invoice

![Invoice](images/sample-invoice.png)

### Structured Expense Data

![Expense Data](images/structured-expense-data.png)

### Processed Folder Automation

![Processed Folder](images/processed-folder.png)

---

## Example Extracted Fields

- Vendor
- Receipt ID
- Date
- Amount
- Currency
- Category
- Expense Type
- Payment Method
- Tax Information

---

## Folder Structure


Unprocessed/
Processed/
Errors_Folder/


---

## Setup Instructions

1. Import the workflow JSON into n8n
2. Configure Google Drive credentials
3. Configure Google Sheets credentials
4. Add OpenAI API credentials
5. Add Google Vision OCR API key
6. Update folder IDs and Sheet IDs
7. Activate workflow

---

## Future Improvements

* Duplicate invoice detection
* Vendor analytics dashboard
* Expense visualization
* Email receipt ingestion
* Multi-language OCR support
* Fraud detection

---

## Author

Pratham Diwakar

````

