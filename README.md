# Sponsor Deal Desk - configuration

Read-only settings for the Sponsor Deal Desk n8n agent. n8n reads these files on every run.

| File | What it holds |
| --- | --- |
| `config/sdd_terms.json` | The creator's terms: floor rules, red lines, auto-send switches |
| `config/sdd_rate_table.json` | Price per 1,000 views and floor per deliverable, with sources |
| `config/sdd_sponsors.json` | Known brands, their official domains and deal history |

Each file is a JSON array with one object per row. Keep every value as text (in quotes) and keep the column names unchanged, or the agent will escalate every offer.

Logs (decisions and creator actions) are not stored here; they stay in n8n Data Tables.
