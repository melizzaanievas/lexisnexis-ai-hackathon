# ⚖️ Protégé: Scenario-to-Authority Educational Engine
> **LexisNexis AI Hackathon 2026** | **Jurisdiction:** Hong Kong SAR  
> **Team:** Prompt to Practice  
> **Live Demo Dashboard:** [https://melizzaanievas.github.io/lexisnexis-ai-hackathon/](https://melizzaanievas.github.io/lexisnexis-ai-hackathon/)

---

## 📌 Executive Summary

Translating complex Hong Kong statutory frameworks and case precedents into simple, accessible materials for legal clinics, law students, and non-lawyers is time-consuming. While AI tools can assist, generic LLMs risk legal inaccuracy, and specialized legal drafting tools often fail to output layperson-friendly formats.

The **Scenario-to-Authority Educational Engine** utilizes **LexisNexis Protégé** to transform primary legal authorities into structured educational hypotheticals, plain-English client takeaway cards, and clinical exercises[cite: 2, 3].

---

## 💡 The Problem & Strategy Pivot

### 1. Initial Challenge & Pivot (Week 2–3)
Our initial concept aimed to use Protégé for automated legal document drafting. However, testing revealed two major bottlenecks:
* **Legal Reasoning Limitations:** Raw legal drafting faced precision issues in legal reasoning.
* **Enterprise Data Confidentiality:** Law firms and in-house counsel faced compliance constraints regarding uploading sensitive client information[cite: 2].

### 2. The Educational Solution
We pivoted to an **Educational & Clinical Scenario Generator**[cite: 2]. By relying on **public Hong Kong precedents** (e.g., Hong Kong Court of First Instance judgments) and anonymized factual patterns, we completely resolved data privacy barriers while targeting high-impact educational workflows[cite: 2].

---

## 🧪 Empirical Testing & Findings (Protégé)

We tested Protégé against the **Hong Kong Employment Ordinance (Cap. 57 Section 9)** using a real-world scenario: an employee fired summarily for uploading 50GB of personal photos to company cloud storage[cite: 2, 3].

### Key Findings:
1. **Drafting Feature Limitation:** Protégé’s native **Draft** module strictly enforces standard legal document types (memos, contracts, letters) and rejects custom educational output requests ("Format not yet supported")[cite: 1, 3].
2. **Conversational Scaffolding Workaround:** Switching to a **two-step conversational workflow** in the **Ask** module successfully retrieved exact primary authorities (*Tsang Tak Chi v China Wall Ltd* [1999]) and reformatted the dense legal analysis into clean educational display cards[cite: 2, 3].

---

## 📊 Platform Comparison Matrix

Since competitor tools were restricted to preview modes, we conducted a feature-to-claim benchmark comparing Protégé's tested capabilities against industry standards[cite: 2]:

| Evaluation Metric | Protégé (LexisNexis) [Tested] | Harvey AI (Industry Benchmark) | Gemini Enterprise (General AI Benchmark) |
| :--- | :--- | :--- | :--- |
| **Primary Data Source** | Direct LexisNexis HK CaseBase & Cap. 57 DBs[cite: 2] | Custom fine-tuned LLMs & Azure Vaults | Google Foundation Models & Workspace Drive |
| **Citation Reliability** | **High** (Direct links to primary HK precedents)[cite: 2] | **High** (Internal vault document citations) | **Medium** (Requires explicit web grounding) |
| **Educational Adaptability** | **High** (via 2-Stage Scaffolding Prompts)[cite: 2, 3] | **Medium** (Corporate & M&A memo focus) | **High** (Strong natural language simplification) |
| **Data Privacy Model** | Private Vaults (De-identified inputs recommended)[cite: 1, 2] | Isolated Enterprise SOC2 Vaults | Workspace IAM Boundary (No model retraining) |

---

## 🛠️ Repository Architecture

```text
lexisnexis-ai-hackathon/
├── README.md                           # Project Summary & Key Findings
├── index.html                          # Live Web Dashboard (GitHub Pages)
├── docs/
│   ├── Checkpoint_1.md                 # Initial Concept Proposal
│   ├── Checkpoint_2.md                 # Mid-point Progress & Pivot Report
│   └── Final_Report.md                 # Comprehensive Hackathon Evaluation
├── testing_data/
│   └── protege_test_outputs.md         # Raw Logged Protégé Output Runs
├── templates/
│   └── hk_employment_prompts.md        # Standardized Scaffolding Prompts
└── comparative_analysis/
    └── platform_comparison.csv         # Comparative Dataset
