# AI CV Screening and Recruitment Automation

I built this n8n workflow to process job applications, extract information from submitted CVs, and use AI to compare the candidate's declared experience with the information found in their CV.

## How it works

1. A candidate submits an application form with the position, email address, declared years of experience, and CV file.
2. The workflow extracts text from the uploaded CV.
3. The AI agent reviews the CV timeline and compares it with the experience declared in the form, then prepares a structured screening result.
4. The candidate is routed according to the screening result, such as Rejected, Training Department, or Advanced Recruitment Pipeline.
5. The workflow records the application in Google Sheets and sends the relevant email notifications, including interview-related messages when applicable.

## Main features

- Job application form with CV upload.
- CV text extraction from PDF files.
- Comparison of declared and CV-based experience.
- AI-assisted screening and inconsistency flags.
- Candidate routing to the relevant recruitment path.
- Google Sheets application tracking.
- Automated applicant and interview email notifications.

## Technologies

n8n, Google Gemini, AI Agent, PDF extraction, Google Sheets, Gmail, JavaScript, and n8n Forms.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Gemini, Google Sheets, and Gmail credentials, then review the application form fields, recruitment routing conditions, and email templates before testing with sample CVs.

## Notes

The workflow includes automated candidate routing based on its configured screening criteria. Review the criteria and screening outputs carefully before using the workflow in a real recruitment process.
