# Patent & Competitor Tracker — Biotech Intelligence Monitor

> Automated patent and competitor monitoring for Biotech and Pharma professionals.



![Status](https://img.shields.io/badge/Status-Complete-brightgreen)



---

## What It Does

Automatically monitors PubMed for new patents and competitor research, generates AI summaries, stores in Airtable, and sends email alerts.

- **Patent monitoring** — tracks new patents in your research area
- **Competitor tracking** — monitors competitor publications on PubMed
- **AI summaries** — Groq generates concise summaries per paper
- **Airtable storage** — all results saved with date and metadata
- **Gmail alerts** — automated email with new findings

---

## Tech Stack

| Layer | Tool |
|---|---|
| Automation | n8n workflow |
| Research API | PubMed API |
| LLM | Groq (llama-3.1-8b) |
| Database | Airtable |
| Email | Gmail HTML |

---

## Architecture

```
Scheduled trigger (n8n)
        ↓
PubMed API fetches latest papers
        ↓
Groq AI generates summary per paper
        ↓
Results saved to Airtable
        ↓
Gmail sends alert email
```

---

## Key Features

- Scheduled automatic monitoring
- AI-generated summaries per patent/paper
- Airtable database with full history
- Gmail HTML formatted alerts
- Configurable search keywords

---

## Technical Notes

- Summary path: `item.json.output` (not nested array)
- Date_Published field: Single line text in Airtable
- AI Agent node used for Groq integration

---

*Built by Deman Meshram | BSc Biotechnology + AI Automation*
