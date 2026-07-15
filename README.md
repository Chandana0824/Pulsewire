# Pulsewire — AI-Powered Incident Response Platform (Demo)

A scaled-down, front-end-only demo of an enterprise SRE copilot: real-time
dashboard, infrastructure topology, AI-powered log analysis with root-cause
suggestions, incident timeline, collaborative war room, AI engineering
copilot, and automated RCA report generation.

**This is a UI/UX demo with simulated data** — built to showcase the product
concept and interaction design for an incident response platform, not a
production system. No backend, no real observability data; everything runs
client-side in a single HTML file.

## Run it locally

Just open `index.html` in any browser — no build step, no dependencies.

```bash
git clone https://github.com/<your-username>/pulsewire-demo.git
cd pulsewire-demo
open index.html   # or double-click the file / drag into a browser
```

## Live demo (GitHub Pages)

After pushing, enable GitHub Pages (Settings → Pages → Deploy from branch →
`main` / root) and it'll be live at:
`https://<your-username>.github.io/pulsewire-demo/`

## Features demoed

| Module | What it shows |
|---|---|
| Dashboard | MTTD/MTTR metrics, live alert feed, AI risk forecast |
| Topology | Clickable service graph with live health status |
| Log Analysis | AI-flagged anomalies + root cause with confidence score |
| Incident Timeline | Detection → response → resolution, event by event |
| War Room | Simulated multi-responder chat with an AI agent participant |
| AI Copilot | Ask questions about the incident/infra, canned intelligent answers |
| RCA Report | One-click auto-generated post-incident report |

## What a production version would add

- Real log/metric ingestion (OpenTelemetry, Prometheus, ELK)
- An LLM + vector search over logs/runbooks for actual root-cause inference
- Anomaly detection models for predictive failure detection
- Real chat/collab backend (websockets) instead of scripted messages
- Auth, RBAC, and integration with PagerDuty/Slack/Jira

## Tech

Single-file HTML/CSS/JS. No frameworks, no build tooling — intentionally kept
simple so it's trivial to read, fork, and extend.
