🤖 AI Resume Screening System

📌 Project Title

AI Resume Screening System using ServiceNow and OpenRouter AI

📖 Project Overview

The AI Resume Screening System is a ServiceNow-based application designed to automate the initial screening of candidate resumes.

The system allows HR users to create job requirements and add candidate details with resume attachments. AI analyzes the candidate's resume and compares the extracted information with the requirements of the selected job.

The system evaluates skills, experience, and qualification, generates a match score, and provides a screening decision such as Selected or Rejected along with AI-generated comments.

This project helps reduce manual resume screening effort and provides a faster and more consistent candidate screening process.

---

✨ Features

- 👨‍💼 Job requirement management
- 👤 Candidate management
- 📄 Resume attachment support
- 🤖 AI-powered resume analysis
- 🧠 Skill extraction from resumes
- 🎓 Qualification analysis
- 💼 Experience analysis
- 📊 Candidate-job match score
- ✅ Automatic candidate selection
- ❌ Automatic candidate rejection
- 💬 AI-generated screening comments
- 📋 Screening result tracking
- 🔄 Automated Flow Designer workflow
- 📧 Email notification
- 📊 Screening dashboard/reporting

---

🛠️ Technologies Used

Technology| Purpose
ServiceNow| Application development and data management
Flow Designer| Automation and workflow
JavaScript| Server-side/client-side scripting
OpenRouter AI| AI-based resume analysis
REST API| Communication with OpenRouter AI
ServiceNow Tables| Storing job, candidate and screening data

---

🗃️ ServiceNow Tables

1. Job Requirement Table

This table stores the requirements for each job.

Fields

- Job Title
- Required Skills
- Required Experience
- Required Qualification
- Minimum Match Score

Example Jobs

- Python Developer
- Java Developer
- ServiceNow Developer
- Data Analyst

---

2. Candidate Table

This table stores candidate information and their uploaded resumes.

Fields

- Candidate Name
- Email
- Phone
- Resume Attachment
- Skills
- Experience
- Qualification
- Applied Job
- Status

Candidate Status

- Submitted
- Selected
- Rejected

---

3. Screening Result Table

This table stores the results generated after AI screening.

Fields

- Candidate
- Job Requirement
- Extracted Skills
- Match Score
- Decision
- AI Comments
- Screening Time

---

🤖 OpenRouter AI Integration

The project uses OpenRouter AI to analyze candidate resume information.

The ServiceNow application sends the relevant resume/job information to the AI service through an API request.

The AI analyzes the candidate information and returns structured screening information such as:

- Extracted skills
- Experience
- Qualification
- Match score
- Screening decision
- AI comments

The returned information is then stored in the Screening Result table.

Basic Integration Flow

ServiceNow
    ↓
Candidate Resume
    ↓
Extract Resume Information
    ↓
OpenRouter AI API
    ↓
AI Analysis
    ↓
Skills + Experience + Qualification
    ↓
Match Score
    ↓
Selected / Rejected
    ↓
Store Screening Result

«Security Note: API keys and other sensitive credentials should never be uploaded to GitHub.»

---

🔄 Project Workflow

HR Creates Job Requirement
            ↓
Candidate Record Created
            ↓
Candidate Uploads Resume
            ↓
Screening Process Starts
            ↓
Resume Information Analyzed
            ↓
OpenRouter AI Processes Information
            ↓
Skills / Experience / Qualification Extracted
            ↓
Candidate Compared With Job Requirements
            ↓
Match Score Generated
            ↓
        Decision
       ↙        ↘
  Selected     Rejected
       ↓          ↓
 Screening Result Created
            ↓
      AI Comments Stored
            ↓
       Email Notification
            ↓
       Dashboard Updated

---

⚙️ How the System Works

Step 1 — Create Job Requirement

HR creates a job requirement and enters:

- Job title
- Required skills
- Required experience
- Required qualification
- Minimum match score

Step 2 — Add Candidate

HR creates a candidate record and provides:

- Candidate name
- Email
- Phone
- Applied job

The candidate's resume can be attached to the record.

Step 3 — Start Screening

The screening workflow is triggered after the candidate information is submitted.

Step 4 — AI Resume Analysis

The system processes the resume information and sends the relevant data to OpenRouter AI.

Step 5 — Compare Candidate With Job

The extracted candidate information is compared with the selected job requirements.

The system evaluates:

- Skills
- Experience
- Qualification

Step 6 — Generate Match Score

The system generates a match score based on how well the candidate matches the job requirements.

Step 7 — Generate Decision

The candidate receives a screening decision:

Selected or Rejected

based on the configured minimum match score.

Step 8 — Store Screening Result

The system creates a Screening Result record containing:

- Candidate
- Job
- Extracted skills
- Match score
- Decision
- AI comments
- Screening time

Step 9 — Notification and Dashboard

The workflow can send an email notification and update the screening dashboard with the latest results.

--
