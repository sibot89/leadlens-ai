# LeadLens

### AI-Powered Lead Research & Outreach Automation

LeadLens is an AI-powered workflow built with **n8n** that automates company research, lead qualification, opportunity identification, and personalized outreach.

The goal is to turn a simple list of companies into structured, qualified leads with actionable business opportunities — while keeping a human in the loop before outreach.

---

## 🚀 What It Does

LeadLens takes company information from a Google Sheet and runs it through an automated research and analysis workflow.

The workflow:

1. **Collects company data** from Google Sheets
2. **Researches companies** using web search and external APIs
3. **Analyzes company information** with an LLM
4. **Identifies potential business opportunities** for AI and automation
5. **Scores leads** based on multiple criteria
6. **Generates personalized outreach** based on the identified opportunity
7. **Requests human approval** before proceeding with outreach
8. **Updates lead status** based on the approval decision

---

## 🧠 Lead Scoring

Instead of relying on a single AI-generated score, LeadLens evaluates leads across multiple dimensions:

* **Company Fit**
* **Automation Potential**
* **Growth & Complexity**
* **Opportunity Clarity**

These factors are combined into an overall **Lead Score** that helps prioritize potential leads.

This makes the workflow more useful for identifying leads that are not only a good company fit, but also have a clear and relevant automation opportunity.

---

## 🔍 Opportunity Identification

A key part of LeadLens is identifying **specific business opportunities** rather than simply deciding whether a company is a good lead.

For each company, the AI analyzes the available research and identifies potential areas where AI or automation could provide business value.

Examples include:

* Lead Qualification
* Customer Support Automation
* Workflow Automation
* Data Processing
* Research Automation

The identified opportunity is then used to make the generated outreach more relevant to the company.

---

## ✉️ Personalized Outreach

After a lead is scored and an opportunity is identified, LeadLens generates personalized outreach based on the research.

The workflow provides:

* Email subject
* Personalized message
* Opportunity used as the basis for the message

The outreach step is intentionally separated from the qualification process so that only qualified leads move forward.

---

## 👤 Human-in-the-Loop

LeadLens does not automatically send outreach immediately after generating it.

A **Human-in-the-Loop approval step** allows a user to review the lead before proceeding.

The workflow can then update the lead status based on the approval decision.

This provides an additional control layer before automated outreach.

---

## 🏗️ Workflow Architecture

```text
Google Sheets
      │
      ▼
Company Data
      │
      ▼
Web Research / API
      │
      ▼
AI Company Analysis
      │
      ▼
Opportunity Identification
      │
      ▼
Lead Scoring
      │
      ▼
Outreach Generation
      │
      ▼
Human Approval
      │
      ├── Reject → Update Status
      │
      └── Approve → Continue Workflow
```

---

## 🛠️ Tech Stack

* **n8n** — Workflow automation
* **Python** — Supporting development and experimentation
* **LLMs** — Company analysis, opportunity identification, scoring, and outreach generation
* **Serper API** — Web research
* **Google Sheets** — Lead input and data storage
* **Structured Outputs** — Reliable AI-generated data
* **Human-in-the-Loop** — Approval workflow

---

## 📊 Example Workflow

A typical lead moves through the following stages:

```text
Company
   ↓
Research
   ↓
AI Analysis
   ↓
Opportunity
   ↓
Lead Score
   ↓
Outreach
   ↓
Human Review
   ↓
Approved / Rejected
```

---

## 🎯 Why LeadLens?

Traditional lead generation often requires manually researching companies, identifying relevant opportunities, qualifying leads, and writing personalized messages.

LeadLens explores how these repetitive tasks can be combined into a single AI-powered workflow while keeping human judgment where it matters.

The project is also designed to be extended with additional research sources, scoring criteria, CRM integrations, and automation steps.

---

## 📸 Screenshots

### Main Workflow

*Add workflow screenshot here.*

### Lead Scoring

*Add lead scoring screenshot here.*

### Human Approval

*Add HITL screenshot here.*

---

## 🔮 Future Improvements

Potential future extensions include:

* CRM integrations
* Additional research sources
* Automated follow-up workflows
* Duplicate lead detection
* More advanced lead qualification
* Scheduled execution
* Additional specialized research agents
* Analytics and reporting dashboard

---

## 👨‍💻 Project

Built by **Sima Baynaghi** as a practical exploration of AI-powered lead research and business automation.

The project focuses on combining **LLMs, web research, workflow automation, structured AI outputs, and human-in-the-loop decision making** into a practical lead generation system.

