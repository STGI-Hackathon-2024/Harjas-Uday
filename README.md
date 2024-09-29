# FILLBOT

## Objective
This project automates the screening of resumes and inputs candidate details into a Microsoft Form, streamlining the recruitment process for HR teams. 
NOTE: Make sure no other instance of browser is opened in your PC. Make sure to clear your email-attachements file.



Video Link: https://drive.google.com/file/d/1t6lCfoZ6mvIv3jJ5kHaGCPOkqgumZQzj/view?usp=sharing
PPT LINK: https://www.canva.com/design/DAGSFhbn-Fw/gpGKqNEvr45jOd9gb_9_BQ/view?utm_content=DAGSFhbn-Fw&utm_campaign=designshare&utm_medium=link&utm_source=editor

## Main Files
- **Main.xaml**: The main execution file for the project.
- **template.xlsx**: Excel template used for data manipulation and audit reporting.

## Problem Statement
HR teams manually review a high volume of resumes, which is time-consuming and prone to errors. Automating the initial screening phase can significantly reduce time, improve accuracy, and create an audit trail for future reference.

## Scope
- **Input**: Emails with the subject line “STGi | New Hire(s)” containing a PDF form attachment.
- **Output**: Extract candidate details from the PDF, populate a Microsoft Form, and generate an audit report of all processed forms.

## Key Features
1. **Email Fetching and Filtering**
   - Retrieve emails from a specified inbox.
   - Filter emails based on the subject line “STGi | New Hire(s)”.

2. **Attachment Download**
   - Download PDF attachments from filtered emails and store them in a designated folder for processing.

3. **Data Extraction**
   - Use RPA tools and OCR to extract key details (e.g., candidate name, education, skills, years of experience) from the PDF forms.

4. **Microsoft Form Submission**
   - Automatically populate the Microsoft Form with the extracted data.
   - Handle form field variations using dynamic selectors or UI Descriptors.

5. **Audit Report Generation**
   - Generate a detailed audit report logging all submissions processed each day.
   - Store the report in `template.xlsx`.

6. **Daily Email Report**
   - Send an email summarizing all processed items at the end of each cycle, with the audit report attached.

7. **Error Handling and Logging**
   - Implement error handling to manage issues like email retrieval failures or incorrect PDF formats.
   - Maintain detailed logs for error tracking, processed items, and system performance.

## Tools & Technologies
- **RPA Platform**: UiPath
- **Programming Languages**: Python, Java
- **Email Integration**: Outlook, Gmail
- **Data Manipulation**: Microsoft Excel
- **Form Automation**: Microsoft Forms
