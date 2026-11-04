# A short code walkthrough

Three places to start if you are reviewing my work for a full-stack role. Each link opens the implementation or its tests.

## 01 · From voice input to a confirmed sale

**Qadam Business** · TypeScript / React / Python

1. Start in the [sale screen](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/web/src/features/voice/Sale.tsx). The seller can review what the app understood before committing a financial entry.
2. Follow the [draft service](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/api/app/services/drafts.py). Preparing a draft and posting money are distinct operations.
3. Read the [draft tests](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/api/tests/test_drafts.py). Look for `test_concurrent_confirmations_consume_once` and `test_ai_failure_preserves_manual_entry`: an impatient double-click and an unavailable model are both normal things to design for.
4. The [ledger tests](https://github.com/foxfordkz-cyber/qadamx-taraz/blob/main/apps/api/tests/test_ledger.py) cover concurrent repayments, reversal history and isolation between businesses.

[Try Qadam Business](https://qadamx-taraz.pages.dev/)

## 02 · A forecast and an observation are different records

**Green Pavlodar** · TypeScript

A planner estimates the future of a site. An inspection later shows what happened. Replacing the prediction with the observation would make the original decision impossible to evaluate.

The [outcomes integration tests](https://github.com/foxfordkz-cyber/qadamxpavlodar/blob/codex/coordinator/apps/server/tests/outcomes.test.ts) exercise that distinction over HTTP: a saved forecast stays fixed, an observation from another site is rejected, and a committed inspection is still available after the server restarts.

[![Green Pavlodar decision lab](https://raw.githubusercontent.com/foxfordkz-cyber/qadamxpavlodar/codex/coordinator/docs/decision-lab/screens/lab-1280.png)](https://green-pavlodar-mock.pages.dev/)

## 03 · What happens when a model is unavailable?

**TeamTrustGate** · Python

Before proposing a Jira ticket, the bot looks for an existing one. The [deduplicator](https://github.com/foxfordkz-cyber/teamtrustg/blob/main/deduplicator.py) checks candidates from Jira and can fall back to comparing word sets. The [scoring code](https://github.com/foxfordkz-cyber/teamtrustg/blob/main/scorer.py) calculates priority in Python. The user gets a preview before a new ticket is created.

[Back to my profile](https://github.com/foxfordkz-cyber)
