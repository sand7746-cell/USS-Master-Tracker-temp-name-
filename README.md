## USS Funding Request Tracker**
An automated tracker for additional funding requests that manages approval workflows and reimbursement processes for student organizations. Built with Google Apps Script and Google Sheets, it streamlines the movement of requests through multiple approval stages and improves tracking accuracy.


## How it Works
Workflow Overview:
Student submits a funding request (Excel or Google Sheet).
The script pulls new request files from a designated Box folder and logs them into a Master Tracker Sheet.
Requests move through multiple approval phases: Finance Committee (FC) and USS (Undergraduate Student Senate).
Emails are automatically sent to the student at key stages (approval, denial, reimbursement/transfer).
The system updates request status and ensures all approvals are tracked.

## Master Approval Home Page
![ApprovalHomePage](https://github.com/user-attachments/assets/c9c6518d-712b-43e8-a7be-e11521721e17)

## Process Flow
<img src="https://github.com/user-attachments/assets/3eba916a-8ed2-444b-b234-30007a508cdd" alt="Reimbursement Flowchart" width="500"/>

## Key Apps Script Features / Formulas:
- **DriveApp.getFolderById()** and **SpreadsheetApp.openById()** to pull files and interact with spreadsheets.

- **IMPORTRANGE()** formulas to dynamically pull values from request sheets into the tracker:

- Custom menu in Sheets with functions like **approveFCRequest(), approveUSSTransfer(), and processCompleted()** for one-click approvals.

<img width="400" height="264" alt="Captura de Pantalla 2025-11-26 a la(s) 19 50 07" src="https://github.com/user-attachments/assets/192e351c-21aa-483e-a614-b4cc7935f0c5" />


- **GmailApp.sendEmail()** to notify students of approvals, denials, or reimbursement status.

- Excel-to-Google Sheet conversion function: **convertExcelToSheet()** ensures compatibility.

<img width="400" height="443" alt="Captura de Pantalla 2025-11-26 a la(s) 19 51 12" src="https://github.com/user-attachments/assets/96f1ee1e-8451-4d96-91f4-489b189c40ad" />

- Unique ID generation for each request: **REQ-2025-XXXX**.

## Results / Impact
- **Time Savings:** Automates tracking and notifications, saving 2-5 hours per week for the Finance Committee depending on request numbers.
- **Accuracy Improvements:** Reduces errors from manual copy-paste, ensures 100% of requests are logged/ updated/ reimbursed consistently.
- **Transparency:** Students can view request status via the tracker link; the automated system enforces approval workflow rules.
- **Flexibility:** Handles Excel and Google Sheet submissions seamlessly.
