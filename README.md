# Patent & Competitor Tracker — Biotech Intelligence Monitor

## 🎬 Demo Video
[▶ Watch Demo on YouTube](https://youtu.be/BePvFlMDYFE)

---

> Automated patent and competitor monitoring for Biotech and Pharma professionals.



![Status](https://img.shields.io/badge/Status-Complete-brightgreen)



---

## The Problem

Biotech companies lose competitive advantage when they miss new patents or competitor publications. Manually checking PubMed every day for new patents and competitor research is time-consuming and easy to forget.

Missing a competitor's patent filing can cost a company millions.

---

## The Solution

Patent & Competitor Tracker automatically monitors PubMed on a schedule, generates AI summaries of new findings, stores everything in Airtable, and sends email alerts — so nothing is ever missed.

- Zero manual effort — runs automatically on schedule
- AI summaries so you understand findings instantly
- Full history stored in Airtable for reference
- Gmail alerts delivered directly to your inbox

---

## Time & Effort Saved

| Task | Manual | This Automation |
|---|---|---|
| Checking PubMed daily | 30-60 mins/day | Zero — fully automatic |
| Reading & summarizing papers | Hours | AI summary in seconds |
| Storing findings | Manual spreadsheet | Auto-saved to Airtable |
| Getting alerts | Not possible | Instant Gmail notification |

---

## Final Output

- ✅ AI-generated summary per new patent/paper
- ✅ All results stored in Airtable with date and metadata
- ✅ Gmail HTML alert with new findings
- ✅ Full searchable history in Airtable database

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
