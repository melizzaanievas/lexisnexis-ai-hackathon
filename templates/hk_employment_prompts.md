# Standardized Conversational Prompt Framework
> **Purpose:** Reusable Two-Stage Scaffolding Prompts for Legal Scenario & Authority Generation

This framework uses a two-stage conversational workflow in the **Ask** module of LexisNexis Protégé to bypass native drafting output constraints and produce plain-English teaching materials grounded in primary legal authorities.

---

## Stage 1: Legal Search & Primary Authority Retrieval

**Goal:** Ground the legal analysis in primary statutes, judicial precedents, and specific jurisdictional standards.

### Prompt Template:
> "An employee at a [JURISDICTION, e.g., Hong Kong] [INDUSTRY TYPE, e.g., financial / retail / logistics] firm [DESCRIBE EMPLOYEE ACTION OR INCIDENT]. The employer terminated them immediately on the spot without notice or payment in lieu. Under [SPECIFIC STATUTE / SECTION, e.g., Section 9 of the HK Employment Ordinance (Cap. 57)] and relevant [JURISDICTION] case precedents, analyze whether this satisfies the legal threshold for summary dismissal. Direct legal authorities required."

---

## Stage 2: Educational Scaffolding & Clinical Display Card Generation

**Goal:** Simplify the Stage 1 legal analysis into plain-English teaching assets for students, clinics, and laypersons without losing statutory precision.

### Prompt Template:
> "Take your legal analysis above and reformat it for a university legal clinic display board. Generate:
> 
> 1. **The Scenario Card:** A 3-sentence plain-English story describing a fictional worker named [NAME] who [BRIEF SUMMARY OF ACT] and got fired.
> 2. **The Verdict:** A 2-bullet summary explaining why the facts might constitute '[HIGH-THRESHOLD VIOLATION, e.g., Gross Misconduct]' vs. '[LOW-THRESHOLD DEFENSE, e.g., Minor Negligence]' under [PRIMARY RETRIEVED PRECEDENT].
> 3. **Clinical Exercise:** 2 quick True/False questions testing key statutory principles for law students."

---

## Stage 3: Multi-Scenario Parallel Generator (Optional)

**Goal:** Generate parallel hypotheticals across different industries to help students see how the same legal principle applies to varied factual contexts.

### Prompt Template:
> "Using the legal framework of [STATUTE / SECTION] and the judicial principle from [LEADING PRECEDENT] (distinguishing [PRIMARY LEGAL TENSION]), generate two NEW, distinct educational hypothetical scenarios set in different industries:
> 
> - **Scenario 1 ([INDUSTRY A]):** [BRIEF FACTUAL SETUP A]
> - **Scenario 2 ([INDUSTRY B]):** [BRIEF FACTUAL SETUP B]
> 
> For EACH scenario, provide:
> 1. A 3-sentence plain-English Scenario Card.
> 2. A dual-verdict analysis explaining [LEGAL ISSUE A] vs. [LEGAL ISSUE B].
> 3. A 1-sentence takeaway card for a non-lawyer employee."
