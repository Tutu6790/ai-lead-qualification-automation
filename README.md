# AI-Powered Lead Qualification Automation

An AI-powered workflow built with **n8n** to automate lead research, qualification, and routing.

## Overview

This project automates the process of evaluating incoming leads to determine their potential suitability for a business's products or services.

It combines workflow automation with AI to help research companies, assess potential fit, explain qualification decisions, and organize leads for follow-up.

## How It Works

1. **Lead Input:** New leads are received through Google Sheets.
2. **Company Research:** The workflow gathers information about the company using its configured research capabilities.
3. **AI Qualification:** AI evaluates the company's potential fit based on the available information.
4. **Decision Making:** The lead is categorized according to the qualification result.
5. **Lead Routing:** The lead is sent to the appropriate spreadsheet.
6. **Notifications:** Qualified leads trigger a notification to the sales team when configured.

## Lead Categories

- **Qualified Leads:** Leads with evidence of potential product or service fit, including the reasons for qualification and recommended follow-up.
- **Flagged Leads:** Leads that appear unlikely to be a good fit, with reasons recorded.
- **Needs Review:** Leads requiring human assessment because the available information is insufficient or the result is uncertain.

## Technologies Used

- **n8n** — Workflow automation
- **AI** — Company assessment and lead qualification
- **Google Sheets** — Lead input and results management
- **Notification integration** — Sales alerts, if configured

## Key Features

- Automated lead processing
- AI-assisted company research and qualification
- Structured qualification reasoning
- Conditional routing based on lead quality
- Human review for uncertain cases
- Automated notifications for qualified leads, if enabled

## Workflow

```text
Incoming Leads
      |
      v
Company Research
      |
      v
AI Lead Qualification
      |
      v
Qualification Decision
      |
      +------------------+
      |         |        |
      v         v        v
  Qualified   Flagged  Needs Review
      |         |        |
      v         v        v
 Notification  Record   Human Review
```

## Project Goals

The goal of this project is to reduce repetitive manual work, improve consistency in lead qualification, and help sales teams prioritize potential opportunities.

## Future Improvements

- Improve research accuracy and evidence collection
- Introduce product-specific fit scores
- Enhance error handling and retry logic
- Track qualification accuracy and workflow performance
- Integrate with CRM platforms

## Project Status

Built as a practical project to explore AI integration, workflow automation, and intelligent lead qualification using n8n.
