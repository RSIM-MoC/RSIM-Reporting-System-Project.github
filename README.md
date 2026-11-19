# RSIM Research Intelligence and Statistical Information Management System
<img width="738" height="387" alt="JJJ" src="https://github.com/user-attachments/assets/d7118b55-71d8-4d4f-98d8-f1b46285a457" />



RSIM reporting system , analyses mid year and end of year reports by removing manual reporting processes to improve  institutional reporting efficiency, strengthen data accuracy and accessibility, and establish a central repository of reliable information to support research, monitoring and evidence-based decision-making within the Ministry. 

## The Problem

RSIM receives periodic reports from 7 Ministry directorates and 11 agencies (e.g. NCA, NITA, CSA, GIFEC), mostly as scattered PDF/Word documents via email attachments. Extracting statistics, standardizing against templates, KPIs, and compiling composite reports is slow which can lead to manual and error-prone and time consumption.

## Objectives

- Receive and track mid-year and end-of-year reports in one place
- Extract achievements, activities, challenges and statistics automatically
- Verify all extracted data with human review before it is used
- Generate composite reports and presentations with minimal manual work
- Build a trusted central repository for research and evidence-based decisions

## Features

| Module | What it does |
|---|---|
| **Submission Portal** | Role-based upload and tracking of agency and directorate reports, with deadline reminders |
| **AI Document Processing** | Parses PDF/Word files, extracts key content and statistics, and summarises per agency, with links back to the source |
| **Verification Centre** | Reviewers compare extractions to the source and approve, edit or reject; only approved data enters the repository |
| **Composite Report Generator** | Merges approved content and charts into a publication-ready report (Word/PDF export) |
| **AI Research Assistant** | Answers plain-language questions about approved institutional documents, with citations |
| **ICT Sector Statistical Dashboard** | Visualises approved indicators by agency, sector and period |
| **Presentation Generator** | Creates branded PowerPoint slides from approved reports and statistics |

## Workflow

1. RSIM opens a reporting period and sets deadlines and templates
2. Focal persons upload reports through the portal
3. The system extracts content and statistics
4. RSIM staff verify and approve extracted items
5. Approved data feeds the repository and dashboard
6. The composite report is generated and reviewed by the RSIM Director
7. Reports and presentations are exported for the Minister, Chief Director, Parliament and NDPC

## User Roles

Administrator (RSIM), Each Agency Focal Person, Each directorate Focal Person, with role-based permissions and full audit logging.

## Proposed Tech Stack

Final choices to be confirmed with the Ministry's IT and security requirements.

- **Front end:** React or similar
- **Back end:** Python (FastAPI or Django)
- **Database:** PostgreSQL
- **Document processing:** PDF/Word parsers with OCR for scanned files
- **AI layer:** LLM with retrieval-augmented generation
- **Hosting:** Ministry-approved or government-compliant

## Implementation Phases

1. Requirements and design
2. Core build (portal, roles, database)
3. AI extraction and verification
4. Reporting and analytics
5. Assistant and presentations
6. Testing and pilot
7. Deployment and training

## Recommendations

1. **Prefer structured KPI entry** (forms or standard templates) over extracting numbers from free-form documents; use AI extraction mainly for qualitative content.
2. **Keep humans in the loop.** Nothing reaches an official report or the dashboard without staff verification and a link to its source.
3. **Settle data governance early:** hosting, access control, and whether documents may be sent to external AI services.
4. **Start narrow.** Begin with the portal plus structured KPI capture and verification for a few agencies, then add AI summarisation, dashboard, assistant and presentations.

## Key Risks

- Inconsistent or scanned report formats reduce extraction accuracy
- Incorrect AI output reaching official reports
- Data privacy and confidentiality (aligned with Ghana's Data Protection Act, 2012, Act 843)
- Low agency adoption and limited team time

## Team

RSIM NSP Project Team, MoCDTI.

