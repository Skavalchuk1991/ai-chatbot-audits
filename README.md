# 🤖 AI Chatbot Audits

Open-source framework for evaluating AI chatbots in production — focused on e-commerce platforms.

## What is this?

A structured evaluation framework for testing AI-powered chatbots across 5 key dimensions:

- **Core Functionality** — Can it do what it's supposed to do?
- **Hallucination Resistance** — Does it make things up?
- **Edge Cases & Robustness** — How does it handle unexpected inputs?
- **Safety & Boundaries** — Is it secure and well-guarded?
- **User Experience** — Is it actually helpful?

Each audit uses **25 standardized test scenarios** with a scoring system (Pass / Partial / Fail) producing a final score out of 100.

## Audit Reports

| Company | Score | Rating | Date | Report |
|---------|-------|--------|------|--------|
| H&M | 76/100 | Good | Mar 2026 | [Full Report](reports/hm-chatbot-audit-2026-03.md) |

## Evaluation Framework

- [AI Chatbot Audit Checklist (25 tests)](framework/ai-chatbot-audit-checklist.md) — ready-to-use template for auditing any e-commerce chatbot

## Key Findings (H&M)

🔴 **Cannot recommend products** from own catalog — sends users to "browse the website"

🔴 **No human agent handoff** — users get stuck in a bot loop with no exit

🟠 **Geographic ambiguity** — "Georgia" interpreted as US state, not country

🟢 **Strong hallucination resistance (90%)** — did not invent products, prices, or policies

🟢 **Strong safety guardrails (90%)** — resisted prompt injection, jailbreak, and abuse

## Methodology

- Manual black-box testing from a customer perspective
- 25 test scenarios across 5 categories
- Scoring: Pass (4 pts) / Partial (2 pts) / Fail (0 pts)
- Rating: 90-100 Excellent | 70-89 Good | 50-69 Needs Improvement | 30-49 Poor | 0-29 Critical

## About

Created by **Siarhei Kavalchuk** — QA Engineer & AI Quality Specialist

- 4+ years in software QA (cross-platform testing, Agile/Scrum)
- AI Evaluation Analyst (RLHF, LLM testing, red teaming)
- Building tools and frameworks for AI quality assurance

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/siarhei-kavalchuk-8a2b30217/)

## License

MIT License — free to use, modify, and distribute.

## Contributing

Found a chatbot worth auditing? Have suggestions for new test scenarios? Open an issue or submit a PR!
