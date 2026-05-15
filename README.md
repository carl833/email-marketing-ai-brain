# Klaviyo AI Brain
> An self-updating AI knowledge base for Klaviyo email marketing strategy

## What it does
A living knowledge base that answers Klaviyo strategy questions 
using AI — automatically updated with the latest Klaviyo 
platform changes, best practices, and industry insights.

Accessible via a Slack slash command, routed through a 
classification layer that determines response complexity 
and selects the appropriate AI model.

## How it works
1. **RSS Digest (automated)** — Make.com scenario fetches 
   the latest Klaviyo blog content on a schedule and writes 
   updates directly to brain.md via GitHub API
2. **Slack Integration** — Slash command triggers a Make.com 
   webhook that routes the question through AI classification
3. **Model Routing** — Simple/factual questions → Gemini Flash, 
   Complex strategy questions → Claude Sonnet
4. **Response** — Answer delivered back to Slack in seconds

## Tech Stack
- **Automation:** Make.com
- **AI Models:** Google Gemini Flash, Anthropic Claude Sonnet
- **Knowledge Base:** GitHub (brain.md, auto-committed on schedule)
- **Interface:** Slack slash command
- **Data Source:** Klaviyo RSS / blog feed

## Key Features
- Self-updating — no manual maintenance required
- Model routing based on question complexity
- Commit history reflects real-time knowledge base activity
- Built specifically for Klaviyo email marketing agency ops

## Status
Internal tool — actively used in production.
