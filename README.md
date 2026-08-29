# ⚖️ LexisNexis Protégé: Scenario-to-Authority Educational Engine

> **LexisNexis AI Hackathon 2026 Submission**  
> **Author & Creator:** Melizza Anievas ([GitHub](https://github.com/melizzaanievas) | [LinkedIn](https://www.linkedin.com/in/melizza-anievas/))  
> **Jurisdiction:** Hong Kong SAR & Universal Statutory/Precedent Frameworks  
> **Live Demo Dashboard:** [melizzaanievas.github.io/lexisnexis-ai-hackathon](https://melizzaanievas.github.io/lexisnexis-ai-hackathon/)

---

## 📌 Project Overview

The **Scenario-to-Authority Educational Engine** bridges the gap between high-precision legal database research and plain-English educational assets. Designed for university legal clinics, non-lawyer client advisories, and corporate stakeholder briefings, this project leverages **LexisNexis Protégé** to transform complex statutory frameworks and judicial ratios into structured, interactive display cards and presentation decks.

---

## 🚀 Key Features & Capabilities

* **Pinpointed Statutory & Precedent Extraction:** Locates and quotes the exact statutory sub-clause (e.g., Cap. 57 s.9(1)(a)(ii), Cap. 486 DPP4(1), Cap. 26 s.12(1)) and judicial ratio (*Tsang Tak Chi v China Wall Ltd*) anchoring a legal dispute.
* **Dual-Audience Output Engine:** Simultaneously generates technical analysis for law students/practitioners and simplified 3-bullet takeaway cards for non-lawyer clients.
* **Universal Vault Scaffolding (`universal_clinic_template_framework.txt`):** Stores reusable instructions in a Protégé Vault, bypassing input limits and reducing prompt setup by 70%.
* **Word/PDF Live Ingestion Bridge:** Resolves enterprise document export constraints by providing a live text ingestion parser on `index.html` that converts copied text into styled display cards.
* **Multi-Format Presentation Exporter:**
  * **📊 One-Click Editable Slides (`.pptx`):** Generates 16:9 widescreen presentation decks (via `PptxGenJS`) that open directly in Google Slides or Microsoft PowerPoint.
  * **✨ Google Apps Script Engine:** Automates slide creation in Google Drive via REST API.
  * **🖨️ PDF Print Engine:** Clean CSS `@media print` formatting for physical handouts and PDF exports.
  * **📋 Clipboard Outline:** Instant slide outline generator for rapid lecture notes.

---

## 🧪 Empirical Test Summary (Test Runs 1 – 8)

| Test Run | Feature / Focus | Objective & Findings |
| :--- | :--- | :--- |
| **Run 1** | Native Draft Module vs. Ask | Confirmed Draft module enforces standard legal memos; Ask tab successfully retrieved Cap. 57 s.9 cases (*Tsang Tak Chi*, *Wan Hung Shu*). |
| **Run 2** | Conversational Scaffolding | Proved two-stage prompts successfully convert raw memo outputs into 3-card plain-English clinical display boards. |
| **Run 3** | Multi-Industry Scaling | Tested parallel scenario generation across Finance (Cloud), Hospitality (Printer), and Logistics (Van Usage). |
| **Run 4** | "Generate Template Responses" Skill | Verified that native skills enforce display card structures dynamically using variable slots (`[INDUSTRY]`, `[WORKER_NAME]`). |
| **Run 5** | Universal Vault Integration | Replaced HK-specific rules with a jurisdiction-agnostic Vault file (`universal_clinic_template_framework.txt`) usable across any LexisNexis law. |
| **Run 6** | Line-Level Statutory Pinpointing | Evaluated precise statutory extraction across Employment (Cap. 57 s.9), Data Privacy (Cap. 486 DPP4), and Sale of Goods (Cap. 26 s.12). |
| **Run 7** | Dual-Audience Output Generation | Validated single-pass output generating technical statutory pinpointing alongside a 3-bullet non-lawyer client takeaway card. |
| **Run 8** | Export Format & Web Bridge | Confirmed Protégé sanitizes raw HTML and exports strictly to Word/PDF; implemented the frontend Ingestion Bridge on `index.html` as a solution. |

*Detailed empirical logs are available in [`testing_data/protege_test_outputs.md`](testing_data/protege_test_outputs.md) and the [`experiments/`](experiments/) directory.*

---

## 📂 Repository Structure

```text
.
├── index.html                            # Live interactive dashboard & slide export engine
├── README.md                             # Project documentation
├── testing_data/
│   └── protege_test_outputs.md          # Complete test logs (Runs 1–8)
└── experiments/
    ├── export_ingestion_bridge.md       # Word/PDF export ingestion bridge log
    ├── presentation_export_guide.md     # Print styles & slide outline guide
    ├── editable_slides_engine.md        # Client-side PptxGenJS engine log
    └── disclaimer_and_slide_export.md   # Compliance, disclaimers & creator credits
```

🌐 Live Web Dashboard & Slide Generator Try the live interactive dashboard:

👉 [https://melizzaanievas.github.io/lexisnexis-ai-hackathon/](https://melizzaanievas.github.io/lexisnexis-ai-hackathon/)

How to Use the Live Dashboard: Select a pre-loaded industry scenario (Finance, Hospitality, or Logistics).

Switch between University Legal Clinic View and Non-Lawyer Client View.

Use the Protégé Word/**PDF** Live Ingestion Bridge to paste text exported from Protégé and render custom cards.

Click 📊 Download Editable Slides (.pptx) to download a presentation deck that opens directly in Google Slides or PowerPoint.

⚠️ Legal AI Disclaimer & Terms of Use This dashboard is an educational research tool powered by LexisNexis Protégé and generative AI models. Outputs do not constitute formal legal advice. Lawyers, legal practitioners, and users must independently verify all statutory provisions, case law citations, and legal analyses prior to professional or judicial reliance. The developers and providers disclaim all legal responsibility for actions taken based on generated content.

👤 Author & Acknowledgments Developer: Melizza Anievas ([GitHub](https://github.com/melizzaanievas) | [LinkedIn](https://www.linkedin.com/in/melizza-anievas/))  

Event: LexisNexis AI Hackathon **2026**

Platform: Discover more about enterprise legal AI at [LexisNexis Protégé](https://www.lexisnexis.com/en-hk/products-and-services/online-solution/lexis-plus-protege?gad_source=1&gad_campaignid=24133535899&gbraid=0AAAAA-ENcK1zAYkv8jZgpWtyFAuZPfdAD&gclid=Cj0KCQjwhsrUBhDxARIsAN3AQSfa8iyHEPhnRVxxOIGQ_CfP7pbQU4_BJOARwQS8g3f0X-pm95ZTVf8aAhx0EALw_wcB).
