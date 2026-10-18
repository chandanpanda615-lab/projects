# Chandan Panda — AI & Automation for Accounts, Audit, Tax & Finance

**CA Final student** who builds automation for the accounts and audit work most teams
still do by hand... and runs it on the live books, every day.

🔗 **Live showcase:** https://chandanpanda615-lab.github.io/projects/

The thread across everything: **domain expertise turned into software.** Not generic
scripts — audit methodology, ICAI standards, and tax law encoded into tools that hold
up against messy, real-world data. Everything below is built and in real use unless
marked *in progress*.

> **On confidentiality:** Several tools were built for live audit engagements.
> Descriptions are deliberately generic — no client names, data, or proprietary code.

---

## 📒 Accounting Operations (the day job)

Purchase bills, prepayments, ledgers and assets in NetSuite for a distribution business.
Brand, vendor, customer and hub names and rupee amounts are withheld. Counts are real.

| # | System | What it does | Result | Stack |
|---|---|---|---|---|
| A1 | **Purchase Bill Booking Pipeline** | Supplier invoice PDFs to NetSuite purchase bills: tax read (free text, then Gemini under a budget cap), e-invoice QR check, all-or-nothing gates, booked ledger against double booking | Grew from **1 brand to 8** in Oct 2026, ~2,400 bills/month in scope; first go-live batch of 130 tied to the rupee | Python · PyMuPDF · zxing-cpp · Gemini · SQLite · NetSuite |
| A2 | **Vendor Prepayment Knock-off Bot** | Applies advances to open bills oldest-first (FIFO per hub) on the NetSuite screen, dry run by default | Sep 2026: 808 prepayments, 5 brands, **808/808 reconciled**, FIFO clean on 39 vendors | Python · Playwright |
| A3 | **GRN vs NetSuite Daily Reconciliation** | Hub goods-received lists against bookings, gaps to a per-hub missing-PDF chase list | Open chase items ~79 → 10 in a week | Python · pandas |
| A4 | **Customer Ledger Builder** | Per-customer ledgers from saved searches, checked against the reco and today's NetSuite balance before sending | 3,310 balances tied, zero variance; runs for a colleague with no Python installed | Python · pandas |
| A5 | **FAR Proof, Row by Row** | Each asset addition tied to an AP invoice, its PDF and IT register serials | 194 clean + 14 doubtful of 208, tie-out passed; 691 of 713 IT rows linked | Python · PyMuPDF · Playwright |
| A6 | **ROC Strike-off Notices to Excel** | Scanned notices read by a vision model, every CIN checked against the MCA master locally | 40,553 rows, 130 left for review; 972 pages in < 2 hrs for ~$2.60 | Python · vision LLM |

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

- **Bill-Discounting JV Maker** — bank tracker → NetSuite journal import, JV numbers written back; 260 JVs reconciled one for one (Python · .exe)
- **Oracle Fusion Attachment Downloader** — invoice PDFs when the API refuses SSO (Python · Playwright)
- **Portal PDF Recovery** — late-uploaded invoice PDFs fetched from the distribution portal (Python · REST API)
- **TDS Master vs Income-tax Act 2025** — NetSuite TDS list checked row by row against the new Act (Excel · tax law)
- **AI Work-Journal Generator** — rough notes → structured HTML/PDF work log (Python · Gemini)
- **Smart Prompt Builder (RTDCFF Skill)** — enforces structured prompting (Claude Skills)
- **Leave Reconciliation Script** — HR system vs physical register (Python · pandas)
- **FC Sheet-Mapping Extractor** — index map across Financial Control files (Python · openpyxl)

## 🚧 In Progress

- **Electronics Distributor Booking** (built, not live) — same gates for phone/laptop distributors; open bills wait on GSTIN and vendor-setup decisions
- **CA Inter Prediction Engine** (85%) — predicts high-probability exam questions; finishing MCQ extraction
- **LPG / BBPS Bulk ID Fetcher** (90%) — bulk consumer-ID verification via BBPS APIs
- **GSTR-3B Cell-Address Extractor** (80%) — robust parsing of merged-cell templates
- **Telegram StockWatch Bot** (80%) — vision-model motion alerts to Telegram

---

## What this work demonstrates

- **Real-world data resilience** — merged cells, multi-format files, regional scripts, broken PDFs.
- **Accounting rules as code** — GST slabs, IGST vs CGST+SGST, TDS 194Q, posting periods, FIFO knock-off, a ledger that refuses double booking.
- **Domain logic as code** — CEAVOP assertions, ICAI standards, GST rules, statutory citations.
- **Modern AI engineering** — RAG pipelines, reusable Claude Skills, vision & embedding models.
- **End-to-end delivery** — raw PDF/Excel in → Excel reports, dashboards, decks & alerts out.

📫 chandanpanda615@gmail.com · CA Finalist · Accounts, GST & Finance Automation
