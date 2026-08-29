# Protégé Empirical Test Logs & Output Records

> **Project:** Scenario-to-Authority Educational Engine  
> **Jurisdiction:** Hong Kong SAR & Universal Legal Frameworks  
> **Testing Window:** August 2026  

---

## 📌 Overview & Methodology

This log documents the empirical test runs executed on LexisNexis Protégé during the hackathon to evaluate:
1. Primary legal search precision and statutory citation reliability under HK Law (Cap. 57, Cap. 486, Cap. 26).
2. Format constraint boundaries within native modules (Drafting vs. Ask features).
3. Conversational scaffolding techniques (Search $\rightarrow$ Reformat) to generate plain-English clinical learning cards.
4. Vault and Skill integration for universal, multi-domain, line-level statutory pinpointing.

---

## 🧪 Test Run 1: System Feature Validation & Format Limitations

### Phase 1: Native "Draft" Module Test
* **Goal:** Test if Protégé's native Drafting tab can directly output custom university legal clinic display board materials.
* **Input Prompt:**
  > *"Based on your analysis, generate the following educational materials for a university legal clinic: A 3-paragraph hypothetical case study titled 'The Cloud Backup Dilemma' for undergraduate law students, a 3-bullet plain-English takeaway for a non-lawyer client, and two discussion questions testing relevant HK standards."*
* **Protégé System Response:**
  > *"The format you have requested is not yet supported by Lexis+AI. However, we are progressively increasing the scope of Draft. To generate a draft in the format of a transactional document, letter, email or clause instead, please rephrase your prompt."*
* **Finding & Limitation Log:** The native Draft module strictly enforces traditional legal document formats (memos, transactional clauses, advice letters) and rejects non-standard educational structures.

---

### Phase 2: Two-Step Conversational Scaffolding ("Ask" Module)
* **Goal:** Test primary statutory retrieval and precedent search in the conversational Ask tab.
* **Input Prompt:**
  > *"An employee at a Hong Kong financial firm backed up 50GB of personal family photos onto the firm's private enterprise cloud storage without authorization. The employer terminated them immediately on the spot without notice or payment in lieu. Under Section 9 of the Hong Kong Employment Ordinance (Cap. 57) and relevant HK case precedents, analyze whether this satisfies the threshold for summary dismissal. Direct legal authorities required."*
* **Protégé Output Grounding:**
  * **Statutory Provision:** Identified Cap. 57 s.9 grounds for summary dismissal (wilful disobedience, misconduct inconsistent with due discharge of duties, gross negligence).
  * **Retrieved Precedents:**
    * *Tsang Tak Chi v China Wall Ltd* [1999] 1 HKC 366 (Threshold distinguishing repudiatory gross misconduct from minor errors).
    * *Wan Hung Shu t/a Paris Wan’s Co v Li Chun Yam* [1993] 2 HKC 714 (Onus of proof on employer regarding summary dismissal).
    * *Allidem v Kwong Si Lin* [2006] 1 HKC 252 (Distinction between termination under s.7 vs summary dismissal under s.9).
    * *Wong Kar Gee Mimi v Applied Development Holdings Ltd* [2016] 1 HKC 350 (Summary dismissal as a strong/extreme measure).
* **Finding:** Protégé demonstrated exceptional legal retrieval precision. However, the raw output was structured as a formal legal memorandum, proving the need for a secondary translation layer for non-lawyers and students.

---

## 🧪 Test Run 2: Pedagogical Re-Formatting (Clinical Display Card)

* **Goal:** Test Protégé's ability to simplify its retrieved context into plain-English educational assets.
* **Input Prompt:**
  > *"Take your legal analysis above and reformat it for a university legal clinic display board. Generate:*
  > *1. The Scenario Card: A 3-sentence plain-English story describing a fictional worker named Alex who backed up personal photos to company cloud storage and got fired.*
  > *2. The Verdict: A 2-bullet summary explaining if this breach is 'Gross Misconduct' or just 'Minor Negligence' under Tsang Tak Chi v China Wall Ltd.*
  > *3. Clinical Exercise: 2 quick true/false questions for law students."*
* **Protégé Generated Output:**
  * **The Scenario Card:** Alex, a mid-level employee at a Hong Kong financial firm, backed up 50GB of personal family photos to the firm’s secure enterprise cloud storage without prior authorisation. The company discovered this activity and immediately terminated Alex without giving notice or paying compensation in lieu, claiming the act was gross misconduct. Alex seeks clarification on whether this termination meets the legal requirements for summary dismissal under Section 9 of the Employment Ordinance (Cap. 57).
  * **The Verdict:**
    * **Gross Misconduct:** Under *Tsang Tak Chi v China Wall Ltd* 1 HKC 366, summary dismissal is only justifiable if the act amounts to a repudiation of a fundamental term of the employment contract or demonstrates reckless disregard for trust and fidelity. Given the sensitivity of enterprise cloud storage at a financial firm, the upload might constitute gross misconduct if it caused serious breaches of company security policies or posed material risks.
    * **Minor Negligence:** However, as held in *Tsang Tak Chi*, instant dismissal is an extreme measure akin to "capital punishment". If the company provided no prior warnings or if Alex’s upload was unintentional with insignificant harm, this act could fall short of gross misconduct and instead be classified as minor negligence, not sufficient to justify summary dismissal.
  * **Clinical Exercise:**
    1. Summary dismissal in Hong Kong can only be justified for gross misconduct that undermines fundamental trust within the employment relationship. **(True)**
    2. Employers are always justified in summarily dismissing employees for a single act of negligence, regardless of its impact or intent. **(False)**
* **Finding:** When provided with a two-stage conversational prompt sequence, Protégé successfully outputs structured plain-English clinical cards while maintaining legal grounding.

---

## 🧪 Test Run 3: Multi-Industry Analogous Scenario Generation

* **Goal:** Test if Protégé can generate parallel factual hypotheticals across different commercial industries while consistently applying s.9 Cap. 57 and *Tsang Tak Chi* legal principles.
* **Input Prompt:**
  > *"Using the legal framework of Section 9 of the HK Employment Ordinance (Cap. 57) and the principle from Tsang Tak Chi v China Wall Ltd [1999] 1 HKC 366 (distinguishing repudiatory gross misconduct from minor negligence/errors of judgment), generate two NEW, distinct educational hypothetical scenarios set in different Hong Kong industries:*
  > *Scenario 1 (Hospitality/Retail): A senior restaurant manager prints personal event flyers using the corporate office printer.*
  > *Scenario 2 (Logistics/Transport): A delivery driver uses the company van to transport personal furniture during off-duty hours without prior approval.*
  > *For EACH scenario, provide: A 3-sentence plain-English Scenario Card, a dual-verdict analysis explaining Gross Misconduct vs. Minor Negligence, and a 1-sentence takeaway card for a non-lawyer employee."*

### Results:
* **Scenario 1 (Hospitality - Office Printer Misuse):**
  * **Scenario Card:** Senior manager prints 500 personal event flyers using office equipment without authorization.
  * **Gross Misconduct:** Senior position heightens duty of fidelity; deliberate policy breach undermines integrity.
  * **Minor Negligence:** Isolated incident, minimal financial cost, absence of clear prior warnings.
  * **Takeaway:** Resource misuse can constitute gross misconduct if it breaches trust in leadership roles.
* **Scenario 2 (Logistics - Off-Duty Vehicle Misuse):**
  * **Scenario Card:** Delivery driver uses company van to move personal furniture over the weekend.
  * **Gross Misconduct:** Deliberate disregard of express vehicle usage restrictions in employment contract.
  * **Minor Negligence:** Misunderstanding of policy, off-duty hours, no disruption to business deliveries.
  * **Takeaway:** Off-duty policy breaches can lead to summary dismissal if mutual trust is undermined.
* **Finding:** Protégé dynamically varies factual settings while maintaining consistent legal reasoning across industries.

---

## 🧪 Test Run 4: Native Skill Feature Test ("Generate Template Responses")

* **Feature Tested:** General Legal Skills $\rightarrow$ Generate Template Responses
* **Objective:** Evaluate if native template skills can enforce custom educational display card structures without defaulting to standard legal memos.
* **Jurisdiction & Issue:** HK Employment Ordinance (Cap. 57 s.9) & *Tsang Tak Chi v China Wall Ltd*

### Results & Findings:
1. **Dynamic Parameterization:** Replaced fixed factual triggers (Alex / 50GB Cloud Backup) with reusable variable slots (`[INDUSTRY]`, `[WORKER_NAME]`, `[EMPLOYEE_ROLE]`, `[INCIDENT_ACTION]`).
2. **Template Adherence:** Protégé consistently produced the 3-part layout (Scenario Card, Dual-Verdict, Clinical Exercise) across new industry inputs without reverting to standard memo formats.
3. **Legal Consistency:** Grounding in Cap. 57 s.9 and *Tsang Tak Chi* was correctly adapted to reflect industry-specific risk profiles (e.g., fleet liability in logistics vs. data integrity in finance).

---

## 🧪 Test Run 5: Universal Vault-Augmented Skill Workflow

* **Features Combined:** Universal Vault (`universal_clinic_template_framework.txt`) + General Legal Skill (`Generate Template Responses`)
* **Objective:** Evaluate whether a jurisdiction-agnostic educational template stored in a Vault can allow Protégé to generate clinical display cards across any legal topic in the LexisNexis database.

### Results & Findings:
1. **Jurisdictional Agnosticism:** Generalized the Vault template by replacing HK-specific statutory references with adaptable placeholders (`[PRIMARY_STATUTE_OR_LAW]`, `[PRIMARY_PRECEDENT]`, `[HIGH_THRESHOLD_VIOLATION]`, `[LOW_THRESHOLD_DEFENSE]`).
2. **Multi-Domain Adaptability:** Verified that Protégé can apply the exact same 3-card educational layout to Employment Law (Cap. 57), Data Privacy Law (Cap. 486 / GDPR), and Common Law Breach of Contract (*Hongkong Fir Shipping*).
3. **Session & Prompt Efficiency:** Reduced input prompt size by over 70% during 1-hour memory reset windows, creating a reusable Vault knowledge asset for legal educators.

---

## 🧪 Test Run 6: Universal Pinpoint Extraction Test Across Multiple Laws

* **Features Combined:** Universal Vault (`universal_clinic_template_framework.txt`) + General Legal Skill (`Generate Template Responses`)
* **Objective:** Test whether Protégé can locate and extract the exact statutory line, sub-clause, and judicial ratio across three distinct legal domains in LexisNexis (Employment Cap. 57, Data Privacy Cap. 486, Sale of Goods Cap. 26).

### Empirical Results & Pinpoint Accuracy:
1. **Employment Law (Cap. 57):** Successfully pinpointed Section 9(1)(a)(ii) (*"misconducts himself... inconsistent with due and faithful discharge of duties"*) as the primary statutory anchor.
2. **Data Privacy Law (Cap. 486):** Successfully pinpointed Schedule 1, Data Protection Principle 4(1) (*"practicable steps to protect against unauthorized or accidental access"*) regarding cloud/email leaks.
3. **Sale of Goods Law (Cap. 26):** Successfully pinpointed Section 12(1) (stipulations as to time) and distinguished repudiatory breaches from warranty claims under *Hongkong Fir Shipping*.
4. **Pedagogical Impact:** Proved that Protégé can bridge high-precision statutory line extraction with plain-English clinical display card generation in a single automated workflow.

---

## 🧪 Test Run 7: Dual-Audience Output Test (Statutory Pinpointing + Client Takeaways)

- **Features Combined:** Universal Vault (`universal_clinic_template_framework.txt`) + General Legal Skill (`Generate Template Responses`)
- **Objective:** Evaluate whether Protégé can generate exact statutory line pinpointing for law students alongside a 3-bullet plain-English takeaway card for non-lawyer clients in a single output stream.
- **Domain Tested:** HK Personal Data (Privacy) Ordinance (Cap. 486) DPP4(1)

### Empirical Findings & Multi-Audience Validation:
1. **Statutory Line Extraction:** Accurately quoted Schedule 1, Data Protection Principle 4(1) (*"all practicable steps shall be taken to ensure that personal data... are protected against unauthorized or accidental access"*).
2. **Client Accessibility:** Successfully rendered a 3-bullet plain-English takeaway card explaining basic privacy rules, breach risks, and immediate reporting steps for non-lawyers.
3. **Pedagogical Impact:** Demonstrated that a single Protégé workflow can simultaneously serve university law clinics (technical legal research) and community legal advice centers (layperson public guidance).
   
---

## 📊 Summary of Key Empirical Findings

1. **Precision Grounding & Pinpointing:** Protégé consistently retrieves accurate statutory provisions and pinpoint sub-clauses across varied commercial statutes in LexisNexis.
2. **Pedagogical Scaling:** Protégé dynamically varies factual settings (Finance $\rightarrow$ Hospitality $\rightarrow$ Logistics $\rightarrow$ Healthcare) while maintaining core judicial principles.
3. **Workflow Solution:** Combining a universal template inside a **Vault** with the **Generate Template Responses Skill** bypasses native drafting constraints and eliminates repetitive prompt setup during session timeouts.
