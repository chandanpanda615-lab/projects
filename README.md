# Chandan Panda — AI & Automation for Audit, Tax & Finance

I'm a Chartered Accountant who builds production-grade automation for the work
most finance professionals still do by hand. Over the last few months I've
designed and shipped **27 tools** spanning statutory audit, GST/tax compliance,
AI agents, RAG pipelines, and a few civic and creative side projects.

The thread that connects all of them: **domain expertise turned into software.**
I don't just write Python — I encode audit logic, ICAI standards, and tax law
into systems that hold up against messy real-world data.

> **A note on confidentiality:** Several tools below were built for live audit
> engagements. The descriptions are deliberately generic — no client names,
> data, or proprietary code is published here. Where code is shareable, it lives
> in the linked project folder.

---

## 🔎 Audit & Assurance Automation

The core of my work — encoding audit methodology into repeatable tooling.

| Project | What it does | Stack |
|---|---|---|
| **IFC Test-of-Design File Mapper** | Scans evidence folders, anonymizes client data, and uses AI to map files to control objectives across HR/Payroll, Direct Tax & SOFTEX. | Python · Claude API |
| **Entity-Specific Audit Program Generator** | Parses Risk & Control Matrices across 6 areas (O2C, P2P, H2R, FSCP, PPE, Tax) and generates an Excel workbook tying procedures to SAP T-codes, control IDs & reviewers. | Python · JSON · Excel |
| **RCM Autofill (Claude Skill)** | A persistent AI skill that reads blank Risk & Control Matrices and auto-applies CEAVOP assertions using strict ICAI theory rules. | Claude Skills · Markdown |
| **Audit Walkthrough → SOP Extractor** | Turns messy post-meeting notes into a process narrative, draft SOP, Mermaid.js flowchart, gap list, and starter RCM. | LLM · Mermaid.js |
| **Vendor Master Anomaly Detection** | 28-parameter rule engine over 500–2,000 vendor records — fuzzy matching on names, bank accounts & PANs to flag duplicates, shell companies & missing fields. | Python · pandas |
| **Employee Master & Payroll Audit Tool** | Validates PF/ESIC applicability, UAN–PAN consistency, duplicate codes/Aadhaar/PAN, and reconciles bank accounts to surface ghost-employee fraud vectors. | Python · pandas · Tkinter |
| **Leave Reconciliation Script** | Cross-checks HR system data against physical leave registers to flag unrecorded leaves and discrepancies. | Python · pandas |
| **Apify Due-Diligence Agent** | LangGraph agent node that scrapes annual reports & news into a structured JSON risk profile for audit risk assessment. | LangGraph · Apify · Claude |
| **SmartExcelReader Wrapper** | OO Python class that dynamically locates headers, unmerges cells while keeping values, and decouples fragile file parsing from audit logic. | Python · openpyxl |
| **FC Sheet-Mapping Extractor** | Builds an index map across multiple Financial Control working files for faster fieldwork navigation. | Python · openpyxl · Jupyter |

## 🧾 Tax & GST Automation

| Project | What it does | Stack |
|---|---|---|
| **GST Reconciliation Engine** | Three-way matching (GSTR-1 vs 3B, GSTR-2B vs books) over 700+ invoices/month across .xlsx & .xlsb — cut 4–6 hrs/client to minutes. | Python · pandas · openpyxl |
| **Professional Tax Challan Extractor** | Auto-detects state across 20 Indian states from PDF challans (incl. Gujarati-script translation), cross-checks against payroll liability. Replaced 2–3 days of manual entry. | Python · pdfplumber · deep-translator |
| **GSTR-3B Cell-Address Extractor** | Pulls tax data from heavily-formatted, merged-cell templates using cached cell coordinates — robust where row-iteration breaks. | Python · openpyxl · JSON |
| **CA Research Assistant (Local RAG)** | Grounds tax answers strictly in the Income Tax Act, Companies Act & Standards on Auditing — retrieves exact paragraph citations, no hallucination. | Python · ChromaDB · Gemini embeddings |

## 🤖 AI Agents, Skills & Infrastructure

| Project | What it does | Stack |
|---|---|---|
| **Smart Prompt Builder (RTDCFF Skill)** | A reusable skill enforcing the Role–Task–Don't–Context–Format–Focus framework to keep technical outputs on rails. | Claude Skills |
| **AI Work-Journal Generator** | Expands rough daily notes into a structured, timestamped professional work log auto-saved as HTML & PDF. | Python · Gemini API |
| **Telegram StockWatch Bot** | Watches a webcam feed, captures on motion, runs frames through a vision model, and pushes pilferage/hygiene alerts to Telegram. | Python · OpenCV · Gemini Vision · Telegram API |

## 🎓 EdTech & Exam Intelligence

| Project | What it does | Stack |
|---|---|---|
| **CA Inter Group Prediction Engine** | Pipeline (`syllabus_extractor` → `smart_extractor` → scorer) over 21 PDFs that predicts high-probability questions and outputs an interactive HTML tool + 6-sheet Excel report. | Python · pdfplumber · Gemini · Claude |
| **CMA Inter OMSM Battle-Plan Dashboard** | 9-tab interactive dashboard: topic heatmap, exact-repeat tracker (found 13 repeats across 14 papers), marks split, gap analysis & phased study plan. | Python · HTML/JS |
| **Finance Slide-Deck Builders** | Converts 351-page lecture packets & standards into modern decks (42-slide valuation deck, ~30-slide Ind AS 116 deck). | Python · python-pptx · Tesseract OCR |
| **ICAI Papers Bulk Downloader** | Crawls the ICAI BOS portal & Drive links to bulk-fetch study modules, MTPs, RTPs & PYQs. | Python · requests · BeautifulSoup |
| **Bulk File Organizer** | CLI scripts that rename and sort downloaded exam papers into standardized project folders. | Python · CLI |

## 🌏 Civic, Personal & Creative

| Project | What it does | Stack |
|---|---|---|
| **PMGSY Govt Data Extractor** | Pulls structured road-project & financial data from inconsistently-formatted government PDFs. | Python · pdfplumber · Gemini |
| **LPG / BBPS Bulk ID Fetcher** | Bulk-verifies 50+ consumer IDs against BBPS bill-fetch APIs, sorting eligible vs ineligible into Excel. | Python · BBPS API |
| **Namma Bus Map (Bengaluru)** | Maps-style web app that geocodes locations, finds stops within ~1km, matches overlapping BMTC routes & draws polylines. | HTML/JS · Leaflet · Overpass API |
| **Maati Katha — Brand & Site** | Full brand identity + landing page for an "anti-resort" village-stay business in Sarangada, Odisha. | HTML/CSS · Recraft · Stitch |
| **Batch Photo Description Generator** | Batch-captions village photos (landscape/time/mood) for alt-text & archives, output to CSV + Markdown. | Python · Gemini Vision |

---

## What this portfolio demonstrates

- **Real-world data resilience** — merged cells, multi-format files, regional scripts, broken government PDFs.
- **Domain logic as code** — CEAVOP assertions, ICAI standards, GST matching rules, statutory citations.
- **Modern AI engineering** — RAG pipelines, agentic workflows (LangGraph), reusable Claude Skills, vision models.
- **End-to-end delivery** — from raw PDF/Excel input to Excel reports, HTML dashboards, decks, and alerts.

📫 chandanpanda615@gmail.com
