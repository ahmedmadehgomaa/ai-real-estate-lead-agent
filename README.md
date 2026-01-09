# AI Real Estate Lead Qualification Agent

## Overview
An **Agentic AI system** that autonomously qualifies real estate leads through natural conversation and executes business actions based on internal decision-making.

The agent interacts with users via Telegram, collects structured data conversationally, evaluates lead readiness internally, and automatically:
- Stores qualified leads
- Schedules meetings
- Politely filters out low-intent users

---

## Key Capabilities

### Conversational Data Collection
The agent gathers:
- Property type (Apartment / Villa / Commercial)
- Buy or Rent intent
- New or Resale preference
- First-time purchase status
- Purchase timeline
- Budget range
- Contact information (Name, Email, Phone)

All data is collected naturally without exposing forms or logic.

---

### Internal Lead Scoring (Hidden)
- Each lead is evaluated internally using weighted rules
- Scoring logic is **never exposed to the user**
- Prevents low-quality leads from entering the CRM

---

### Autonomous Decision Making
Based on internal evaluation:
- **High-quality leads**
  - Automatically saved to Google Sheets
  - Meeting scheduled via Google Calendar
- **Low-quality leads**
  - Conversation ends politely
  - No data stored

---

### Agent Tool Usage
The AI agent autonomously uses:
- Google Sheets (CRM storage)
- Google Calendar (meeting scheduling)
- Short-term conversational memory
- External LLM via OpenRouter

---

## Tech Stack
- **n8n**
- **LangChain Agent (n8n)**
- **Telegram Bot**
- **OpenRouter LLM**
- **Google Sheets API**
- **Google Calendar API**

