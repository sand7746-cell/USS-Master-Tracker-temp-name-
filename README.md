## USS Funding Request Tracker**
An automated tracker for additional funding requests that manages approval workflows and reimbursement processes for student organizations. Built with Google Apps Script and Google Sheets, it streamlines the movement of requests through multiple approval stages and improves tracking accuracy.

## Demo
[Insert screenshots or GIFS]

## How it Works
Workflow Overview:
Student submits a funding request (Excel or Google Sheet).
The script pulls new request files from a designated Box folder and logs them into a Master Tracker Sheet.
Requests move through multiple approval phases: Finance Committee (FC) and USS (Undergraduate Student Senate).
Emails are automatically sent to the student at key stages (approval, denial, reimbursement/transfer).
The system updates request status and ensures all approvals are tracked.

## Key Apps Script Features / Formulas:
DriveApp.getFolderById() and SpreadsheetApp.openById() to pull files and interact with spreadsheets.

IMPORTRANGE() formulas to dynamically pull values from request sheets into the tracker:

Custom menu in Sheets with functions like approveFCRequest(), approveUSSTransfer(), and processCompleted() for one-click approvals.

GmailApp.sendEmail() to notify students of approvals, denials, or reimbursement status.

Excel-to-Google Sheet conversion function: convertExcelToSheet() ensures compatibility.

Unique ID generation for each request: REQ-2025-XXXX.

## Results / Impact
**Time Savings:** Automates tracking and notifications, saving 2-5 hours per week for the Finance Committee depending on request numbers.
**Accuracy Improvements:** Reduces errors from manual copy-paste, ensures 100% of requests are logged/ updated/ reimbursed consistently.
**Transparency:** Students can view request status via the tracker link; the automated system enforces approval workflow rules.
**Flexibility:** Handles Excel and Google Sheet submissions seamlessly.
