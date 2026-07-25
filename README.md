# AI Risk Register Template

A reusable, NIST AI RMF-aligned risk register for tracking model risk, data governance gaps, and compliance obligations across an AI product's lifecycle. Built and used to track AI risk for live enterprise SaaS AI modules; adapted here into two forms depending on what you need.

---

## Why this exists

Most AI product teams don't have a working risk register — they have scattered Jira tickets, a compliance spreadsheet nobody updates after the first audit, and no record of a risk once it's shipped. This template gives any team a single, living document that tracks AI-specific risk from design through production, mapped to a framework enterprise customers and auditors actually recognize.

---

## What's in this repo

| File | What it is | Use this when |
|---|---|---|
| [`AI-Risk-Register-Template.xlsx`](./AI-Risk-Register-Template.xlsx) | Full register worked through a realistic enterprise SaaS scenario (multi-tenant RAG assistant, LLM summary generation, AI lead scoring) — 8 pre-filled example risks, in spreadsheet form | You want to see how the register works in practice, or you're evaluating this as a governance work sample. Also usable as a live working file — duplicate the sheet and start tracking your own risks directly in it |
| [`AI-Risk-Register-Template-Universal.pdf`](./AI-Risk-Register-Template-Universal.pdf) | Industry-agnostic version built around 8 universal AI failure patterns instead of one vertical | You're a startup in any industry and want to read through the reasoning and column definitions before building your own version |

Both files use the same 13-column structure, scoring rubrics, and NIST AI RMF mapping — the difference is only in the worked examples and the format each is delivered in.

> **Note on formats:** the SaaS example ships as XLSX because a risk register is meant to be worked in, not just read — open it, duplicate the sheet, and start adding your own rows. The Universal version ships as PDF for readability; if you want to actually use it as a starting template rather than a reference document, copy the column structure into your own spreadsheet or Notion table first.

---

## How the register works

Every risk is:
1. **Mapped to a NIST AI RMF function** — Govern, Map, Measure, or Manage
2. **Categorized** — Data Governance, Model Risk, Compliance, Bias/Fairness, Vendor, or Operational
3. **Scored** on a 5×5 likelihood × impact matrix (1–25), sorted into Low / Medium / High / Critical
4. **Owned** by a named role, with a mitigation action and a review cadence

Critical-tier risk is designed to block release until mitigated or explicitly risk-accepted by a named senior owner — the matrix isn't decorative, it's meant to gate ship decisions.

---

## Quick start

1. Download `AI-Risk-Register-Template.xlsx` and make a copy — this is the working file. Delete the pre-filled example rows once you understand the pattern each one represents.
2. Read `AI-Risk-Register-Template-Universal.pdf` if you want the reasoning behind each column and a set of industry-agnostic risk patterns to start from before writing your own.
3. Add a row every time your product introduces a new model, a new data source, or a new AI vendor.
4. Score using the Likelihood/Impact rubrics included in both files; review Critical/High risks weekly, everything else monthly.
5. Wire it into your existing sprint process — see the "Integrating into Agile Sprints" section in either file.

---

## Frameworks referenced

- **NIST AI RMF** (Govern / Map / Measure / Manage)
- **India DPDP Act 2023** — dedicated section in both files covering cross-border transfer, SDF thresholds, and consent architecture
- General principles applicable alongside **EU AI Act** risk tiering and **ISO 42001** management-system requirements

---

## About

Built by **Anubhav Verma** — AI governance and product strategy practitioner, based in Lucknow, India. This template is part of a broader portfolio applying NIST AI RMF, EU AI Act, and India's DPDP Act to practical, product-team-usable governance artifacts.

[LinkedIn] · [Portfolio] · [Contact]

*Replace the bracketed links above before publishing.*

---

## License

MIT — use, adapt, and redistribute freely. Attribution appreciated but not required.
