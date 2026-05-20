# Make Blueprint Repository

This repository contains exported .json Make blueprint files used to automate workflows and integrations.
The blueprints can be imported directly into Make to review, execute, customize, and extend the automation scenarios.

# Repository Structure

├── blueprints/\
│   ├── scenario-01.json\
│   └── ...\
└── README.md

Each .json file represents a Make scenario blueprint.

# Requirements

Before importing and running the blueprints, ensure you have:

A valid Make account
Configured credentials/connections for:
Microsoft Outlook
Groq AI
Microsoft Excel

Some scenarios may also require additional modules or providers depending on the workflow implementation.

# Importing Blueprints into Make
## 1. Open Make

Access your Make workspace:

Make Platform

## 2. Create a New Scenario

Inside Make:

Click Create a new scenario
Open the scenario menu (...)
Select Import Blueprint

## 3. Upload the Blueprint File

Choose one of the .json files from the repository.
After import, Make will recreate the workflow structure automatically.

# Required Connections

After importing a blueprint, Make will request connection mapping for external services.
You must configure the required providers before the scenario can run successfully.

## Microsoft Outlook

Used for:
- Sending emails
- Reading inbox messages
- Monitoring mailbox events

You will need:
- A Microsoft account
- Outlook/Microsoft 365 authorization inside Make

Reference:
[Microsoft Outlook](https://www.microsoft.com/microsoft-365/excel?utm_source=chatgpt.com)

## Groq AI

Used for:
- AI inference
- Prompt execution
- Text generation
- LLM-powered workflow actions

You will need:
- A Groq API key
- A configured HTTP/API connection inside Make

Reference:
[Groq](https://groq.com?utm_source=chatgpt.com)

## Microsoft Excel

Used for:
- Spreadsheet reading/writing
- Data persistence
- Reporting
- Structured workflow outputs

You will need:
- A Microsoft account
- Access to Excel files stored in OneDrive or SharePoint

Reference:
[Microsoft Excel](https://www.microsoft.com/microsoft-365/excel?utm_source=chatgpt.com)

# Running a Scenario
After configuring all required connections:
- Open the imported scenario
- Review all modules and mappings
- Validate variables, filters, and routes
- Click Run once to test the workflow
- Enable scheduling if continuous execution is required
- Customization

The blueprints are fully editable inside Make.

You can:
- Add or remove modules
- Modify prompts
- Change routing logic
- Replace providers
- Extend integrations
- Adjust scheduling and triggers

# Troubleshooting
## Missing Connections

If modules appear with warnings after import:
- Open the affected module
- Reassign or create the required connection
- Save the scenario again

# Recommended Workflow
1. Import blueprint
2. Configure required connections
3. Validate mappings
4. Execute test runs
5. Enable scheduling/production execution