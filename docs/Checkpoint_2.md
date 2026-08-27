# Checkpoint 2 Submission: Progress, Pivot & Testing
> **Team:** Prompt to Practice
> **Submitted:** August 30, 2026

## Progress and Development
Since Week 2, we pivoted from legal document drafting to an Educational Scenario-to-Authority Engine for legal clinics and students. Drafting failed due to inaccurate legal reasoning and firm confidentiality concerns regarding sensitive client data. By focusing on educational hypotheticals, we resolved privacy barriers using public Hong Kong precedents and de-identified factual patterns.

## Testing Conducted
We tested Protégé using Hong Kong Employment Ordinance (Cap. 57 s.9) scenarios, specifically an employee fired summarily for uploading 50GB of personal photos to company cloud storage. We evaluated outputs using a two-stage prompt structure: first testing legal retrieval precision, then reformatting dense analysis into plain-English scenario cards, dual-verdict takeaways, and true/false clinical exercises verified against primary legal databases.

## Early Findings
Protégé demonstrated high retrieval precision, accurately surfacing leading precedents such as *Tsang Tak Chi v China Wall Ltd*. However, native drafting attempts failed as Protégé rejected non-standard document formats ("Format not yet supported"). A two-stage conversational workflow successfully bypassed this, transforming complex legal analysis into accessible, high-quality clinical cards while preserving statutory accuracy.

## Challenges and Next Steps
Protégé lacks native UI features for legal educators to display clinical scenarios. As a workaround, we built a live, low-code interactive dashboard via GitHub Pages. Moving forward, we will expand our test suite to include additional Cap. 57 topics (such as unlawful wage deductions) and refine our comparative benchmark against Harvey AI and Gemini Enterprise.
