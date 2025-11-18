# gmail-llm-sheets-automation
Automatically ingests incoming Gmail messages, extracts data from attached PDFs, structures it with an LLM (Groq), and appends the results to a Google Sheet.



<img width="1222" height="437" alt="Screenshot 2025-11-17 at 21 05 54" src="https://github.com/user-attachments/assets/5c5ef169-ae49-4b87-96ef-2efd880f4bee" />


--- 

### What this does:

Listen to Gmail for new messages (filter by label/query).
Download PDF attachments and extract text.
Parse & normalize fields with an LLM using a strict schema (structured output).
Append a new row to a target Google Sheet.

### Prerequisites:

Python 3.10+ (or Docker)
Groq API key (for llama-3.x / mixtral / your choice)

Google Cloud project with:
Gmail API enabled
Google Sheets API enabled
Service account JSON creds
A Google Sheet created and shared with the service account email (Editor).
