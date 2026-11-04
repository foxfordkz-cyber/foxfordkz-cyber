<h1>Damir · Full-stack developer</h1>

![TypeScript and Python · Kazakhstan · Open to full-stack roles](assets/full-stack-portfolio.svg)

I build web apps for people working in Kazakhstan. I like the part where the interface meets the database: a seller can correct a voice transcription, retry a payment, or lose their connection without having to guess what was saved.

**Open to full-stack roles with TypeScript and Python.** [Email me](mailto:foxfordkz@gmail.com) · [Browse the code walkthrough](ENGINEERING.md)

## Featured build · Qadam Business

A seller in Taraz says a sale out loud in Kazakh or Russian. The app drafts the entry, the seller checks the customer and amount, and only then does it enter the ledger.

[![Qadam Business seller interface](https://raw.githubusercontent.com/foxfordkz-cyber/qadamx-taraz/main/docs/assets/readme/cabinet.webp)](https://qadamx-taraz.pages.dev/)

**What to look for:** the React screen handles review; the Python API decides whether the draft can be confirmed. If two confirmations arrive together, the tests check that only one sale is recorded.

[Open the app ↗](https://qadamx-taraz.pages.dev/) · [React screen](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/web/src/features/voice/Sale.tsx) · [FastAPI service](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/api/app/services/drafts.py) · [Concurrency tests](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/api/tests/test_drafts.py)

## More selected work

| Project | What to try | Look under the hood |
| --- | --- | --- |
| **[Green Pavlodar](https://github.com/foxfordkz-cyber/qadamxpavlodar)** | [Pick a plot](https://green-pavlodar-mock.pages.dev/), compare planting plans, then explore the 20-year forecast. | [Snapshot and recovery tests](https://github.com/foxfordkz-cyber/qadamxpavlodar/blob/codex/coordinator/apps/server/tests/outcomes.test.ts) show how a forecast survives later inspections and a server restart. |
| **[TeamTrustGate](https://github.com/foxfordkz-cyber/teamtrustg)** | Follow a customer request from Telegram to a reviewed Jira ticket. | [Duplicate detection](https://github.com/foxfordkz-cyber/teamtrustg/blob/main/deduplicator.py) uses a keyword fallback when the model is unavailable. |
| **[Qazaq Loc QA](https://github.com/foxfordkz-cyber/stupits-karaganda)** · team project | [See the editor](https://github.com/foxfordkz-cyber/stupits-karaganda/blob/codex/integration-kit/docs/images/review-overview.jpg) explain a flagged Russian-to-Kazakh translation. | [Team verification script](https://github.com/foxfordkz-cyber/stupits-karaganda/blob/codex/integration-kit/scripts/verify-team.mjs) ties the checks to a reproducible report. |

## Stack in practice

**Frontend** · TypeScript, React  
**Backend** · Python, FastAPI, PostgreSQL  
**Engineering interests** · Bilingual interfaces, API design, transaction safety and integration testing

If your team is building a product with a TypeScript frontend and a Python backend, [let’s talk](mailto:foxfordkz@gmail.com).
