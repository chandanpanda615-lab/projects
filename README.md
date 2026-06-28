# Chandan Panda — AI & Automation for Audit, Tax & Finance

**Chartered Accountant (Finalist)** who builds production automation for the audit
work most firms still do by hand — and runs it on live engagements.

🔗 **Live showcase:** https://chandanpanda615-lab.github.io/projects/

The thread across everything: **domain expertise turned into software.** Not generic
scripts — audit methodology, ICAI standards, and tax law encoded into tools that hold
up against messy, real-world data. Everything below is built and in real use unless
marked *in progress*.

> **On confidentiality:** Several tools were built for live audit engagements.
> Descriptions are deliberately generic — no client names, data, or proprietary code.

---

## ⭐ Selected Work

| # | Project | What it does | Impact | Stack |
|---|---|---|---|---|
| 1 | **GST Reconciliation Engine** | Three-way GSTR-1 vs 3B vs books matching over 700+ invoices/mo | 5 hrs → <30 min per client/mo | Python · pandas · openpyxl |
| 2 | **Audit Program Generator** | RCMs → Q4 program mapping 45 controls to SAP T-codes & reviewers | Replaces manual drafting | Python · JSON · Excel |
| 3 | **Vendor Master Anomaly Detection** | 28-param engine, fuzzy matching on names/banks/PANs | Catches duplicate-payment & fraud risk | Python · pandas |
| 4 | **IFC Test-of-Design Mapper** | AI maps evidence files to control objectives + drafts tests | Compresses ToD evidence phase | Python · Claude API |
| 5 | **Employee & Payroll Audit** | PF/ESIC, UAN–PAN, duplicate/bank checks | Ghost-employee fraud detection | Python · pandas · Tkinter |
| 6 | **RCM Autofill (Claude Skill)** | Encodes CEAVOP/ICAI rules; auto-fills Risk & Control Matrices | Domain logic reused every engagement | Claude Skills |
| 7 | **PT Challan Extractor** | 20-state PDF challan parsing (incl. Gujarati), payroll cross-check | Replaced 2–3 days of data entry | Python · pdfplumber |
| 8 | **CMA OMSM Dashboard** | 9-tab interactive dashboard from 14 papers | Data-eng + front-end range | Python · HTML/JS |
| 9 | **Finance Slide-Deck Builders** | 28-slide DCF & ~30-slide Ind AS 116 decks from dense PDFs | 350-page packets → decks | Python · python-pptx · OCR |
| 10 | **CA Research Assistant (RAG)** *(prototype, 70%)* | Local RAG grounding answers in statute with exact citations | Next: Ollama for client-data safety | Python · ChromaDB · embeddings |

## 🛠️ Also Built & In Use

- **AI Work-Journal Generator** — rough notes → structured HTML/PDF work log (Python · Gemini)
- **Smart Prompt Builder (RTDCFF Skill)** — enforces structured prompting (Claude Skills)
- **Leave Reconciliation Script** — HR system vs physical register (Python · pandas)
- **FC Sheet-Mapping Extractor** — index map across Financial Control files (Python · openpyxl)

## 🚧 In Progress

- **CA Inter Prediction Engine** (85%) — predicts high-probability exam questions; finishing MCQ extraction
- **LPG / BBPS Bulk ID Fetcher** (90%) — bulk consumer-ID verification via BBPS APIs
- **GSTR-3B Cell-Address Extractor** (80%) — robust parsing of merged-cell templates
- **Telegram StockWatch Bot** (80%) — vision-model motion alerts to Telegram

---

## What this work demonstrates

- **Real-world data resilience** — merged cells, multi-format files, regional scripts, broken PDFs.
- **Domain logic as code** — CEAVOP assertions, ICAI standards, GST rules, statutory citations.
- **Modern AI engineering** — RAG pipelines, reusable Claude Skills, vision & embedding models.
- **End-to-end delivery** — raw PDF/Excel in → Excel reports, dashboards, decks & alerts out.

📫 chandanpanda615@gmail.com · CA Finalist · Embedded Audit Automation Specialist
