# Protégé Empirical Test Logs & Output Records 
> **Project:** Scenario-to-Authority Educational Engine   
> **Jurisdiction:** Hong Kong SAR   
> **Primary Statutory Focus:** Hong Kong Employment Ordinance (Cap. 57)   
> **Testing Dates:** August 2026 
 
--- 
 
## 📌 Overview & Methodology 
This log documents all empirical test runs executed on LexisNexis Protégé during the hackathon . Testing was structured to evaluate: 
1. Primary legal search precision and citation reliability under HK Employment Law (Cap. 57) . 
2. Pedagogical reformatting capabilities (converting dense memos into plain-English clinical display cards) . 
3. Format constraint boundaries within native modules (Drafting vs. Ask features)[cite: 1, 3]. 
4. Multi-scenario factual adaptation across different commercial industries . 
 
--- 
 
## 🧪 Test Run 1: System Feature Validation & Format Limitations 
 
### Phase 1: Native "Draft" Module Test 
* **Goal:** Test if Protégé's native Drafting tab can directly output custom university legal clinic materials[cite: 1, 3]. 
* **Input Prompt:**   
  > *"Based on your analysis, generate the following educational materials for a university legal clinic: A 3-paragraph hypothetical case study titled 'The Cloud Backup Dilemma' for undergraduate law students, a 3-bullet plain-English takeaway for a non-lawyer client, and two discussion questions testing relevant HK standards."*  
* **Protégé System Response:**   
  > *"The format you have requested is not yet supported by Lexis+AI. However, we are progressively increasing the scope of Draft. To generate a draft in the format of a transactional document, letter, email or clause instead, please rephrase your prompt."*  
* **Finding & Limitation Log:**   
  The native **Draft** module strictly enforces traditional legal document formats (memos, transactional clauses, advice letters) and rejects non-standard educational structures[cite: 1, 3]. 
 
--- 
 
### Phase 2: Two-Step Conversational Scaffolding ("Ask" Module) 
* **Goal:** Test primary statutory retrieval and precedent search in the conversational **Ask** tab . 
* **Input Prompt:**   
  > *"An employee at a Hong Kong financial firm backed up 50GB of personal family photos onto the firm's private enterprise cloud storage without authorization. The employer terminated them immediately on the spot without notice or payment in lieu. Under Section 9 of the Hong Kong Employment Ordinance (Cap. 57) and relevant HK case precedents, analyze whether this satisfies the threshold for summary dismissal. Direct legal authorities required."*  
* **Protégé Output:**   
  * **Statutory Grounding:** Identified Cap. 57 s.9 grounds for summary dismissal (wilful disobedience, misconduct inconsistent with due discharge of duties, gross negligence) . 
  * **Retrieved Precedents & Cases:** 
    - *Tsang Tak Chi v China Wall Ltd* [1999] 1 HKC 366 (Established threshold distinguishing repudiatory gross misconduct from minor errors) . 
    - *Wan Hung Shu t/a Paris Wan’s Co v Li Chun Yam* [1993] 2 HKC 714 (Onus of proof on employer regarding summary dismissal) . 
    - *Allidem v Kwong Si Lin* [2006] 1 HKC 252 (Distinction between termination under s.7 vs summary dismissal under s.9) . 
    - *Wong Kar Gee Mimi v Applied Development Holdings Ltd* [2016] 1 HKC 350 (Summary dismissal as a strong and extreme measure) . 
    - *Lam Siu Mei v The Hong Kong Society for the Blind*  
    - *Zhang Qiang v Cisco Systems (HK) Ltd*  
    - *Cheung Chi Wah, Patrick v Hong Kong Cement Co Ltd*  
    - *Star Fair Electronics Co Ltd v Wong Tak Cheung & Ors*  
* **Finding:**   
  Protégé demonstrated exceptional legal retrieval precision . However, the initial raw output was structured as a formal legal memorandum, proving the need for a secondary translation layer for non-lawyers and students . 
 
--- 
 
## 🧪 Test Run 2: Pedagogical Re-Formatting (Clinical Display Card) 
 
* **Goal:** Test Protégé's ability to simplify its own retrieved context into plain-English educational assets . 
* **Input Prompt:**   
  > *"Take your legal analysis above and reformat it for a university legal clinic display board. Generate:*   
  > *1. The Scenario Card: A 3-sentence plain-English story describing a fictional worker named Alex who backed up personal photos to company cloud storage and got fired.*   
  > *2. The Verdict: A 2-bullet summary explaining if this breach is 'Gross Misconduct' or just 'Minor Negligence' under Tsang Tak Chi v China Wall Ltd.*   
  > *3. Clinical Exercise: 2 quick true/false questions for law students."*  
 
* **Protégé Generated Output:**   
  * **The Scenario Card:**   
    > Alex, a mid-level employee at a Hong Kong financial firm, backed up 50GB of personal family photos to the firm’s secure enterprise cloud storage without prior authorisation . The company discovered this activity and immediately terminated Alex without giving notice or paying compensation in lieu, claiming the act was gross misconduct . Alex seeks clarification on whether this termination meets the legal requirements for summary dismissal under Section 9 of the Employment Ordinance (Cap. 57) . 
  * **The Verdict:**   
    > - **Gross Misconduct:** Under *Tsang Tak Chi v China Wall Ltd* 1 HKC 366, summary dismissal is only justifiable if the act amounts to a repudiation of a fundamental term of the employment contract or demonstrates reckless disregard for trust and fidelity . Given the sensitivity of enterprise cloud storage at a financial firm, the upload might constitute gross misconduct if it caused serious breaches of company security policies or posed material risks .   
    > - **Minor Negligence:** However, as held in *Tsang Tak Chi*, instant dismissal is an extreme measure akin to "capital punishment" . If the company provided no prior warnings or if Alex’s upload was unintentional with insignificant harm, this act could fall short of gross misconduct and instead be classified as minor negligence, not sufficient to justify summary dismissal . 
  * **Clinical Exercise:**   
    > 1. Summary dismissal in Hong Kong can only be justified for gross misconduct that undermines fundamental trust within the employment relationship. **(True)**    
    > 2. Employers are always justified in summarily dismissing employees for a single act of negligence, regardless of its impact or intent. **(False)**  
 
* **Finding:**   
  When provided with a two-stage conversational prompt sequence, Protégé successfully outputs structured plain-English clinical cards while maintaining legal grounding . 
 
--- 
 
## 🧪 Test Run 3: Multi-Industry Analogous Scenario Generation 
 
* **Goal:** Test if Protégé can generate parallel factual hypotheticals across different commercial industries while consistently applying s.9 Cap. 57 and *Tsang Tak Chi* legal principles . 
* **Input Prompt:**   
  > *"Using the legal framework of Section 9 of the HK Employment Ordinance (Cap. 57) and the principle from Tsang Tak Chi v China Wall Ltd [1999] 1 HKC 366 (distinguishing repudiatory gross misconduct from minor negligence/errors of judgment), generate two NEW, distinct educational hypothetical scenarios set in different Hong Kong industries:*   
  > *Scenario 1 (Hospitality/Retail): A senior restaurant manager prints personal event flyers using the corporate office printer.*   
  > *Scenario 2 (Logistics/Transport): A delivery driver uses the company van to transport personal furniture during off-duty hours without prior approval.*   
  > *For EACH scenario, provide: A 3-sentence plain-English Scenario Card, a dual-verdict analysis explaining Gross Misconduct vs. Minor Negligence, and a 1-sentence takeaway card for a non-lawyer employee."*  
 
* **Protégé Generated Output:** 
 
  ### Scenario 1: Hospitality / Retail (Office Printer Misuse) 
  * **Plain-English Scenario Card:** A senior manager at a high-end restaurant prints 500 personal event flyers using the company printer without asking for permission . The financial cost is minor, but the act breaches the company policy that restricts personal usage of office resources . The manager’s role includes maintaining professional conduct and setting an example for junior staff . 
  * **Dual-Verdict Analysis:**   
    - **Gross Misconduct:** May meet the threshold if it demonstrates intentional misuse of resources, violating essential duties of fidelity and trust . As a senior manager, their actions directly undermine corporate integrity, justifying immediate dismissal under Section 9 .   
    - **Minor Negligence:** Alternatively, if this act is isolated, has minimal financial impact, and there is a lack of clear policy prohibiting such actions, it may not rise to gross misconduct . The manager could face disciplinary measures but retain employment . 
  * **Takeaway Card:** Misusing resources can be gross misconduct if it breaches trust and fidelity, especially for employees in leadership roles . 
 
  ### Scenario 2: Logistics / Transport (Off-Duty Vehicle Misuse) 
  * **Plain-English Scenario Card:** A delivery driver employed by a logistics company uses the company van to move their personal furniture over the weekend without informing the employer . While there’s no disruption to scheduled deliveries, the action breaches the company’s vehicle usage policy outlined in their employment contract . 
  * **Dual-Verdict Analysis:**   
    - **Gross Misconduct:** Using company property for personal use may justify summary dismissal if the driver deliberately ignored clear prohibitions in the employment agreement, signaling a disregard for contractual terms .   
    - **Minor Negligence:** If the driver misunderstood the policy or believed such use was permissible (e.g., no prior warnings and no harm caused), the act could be categorised as a minor error of judgment where disciplinary measures short of dismissal are appropriate . 
  * **Takeaway Card:** Even off-duty breaches of company policy can result in dismissal if they undermine an employment relationship’s trust . 
 
--- 
 
## 📊 Summary of Empirical Findings 
1. **Precision Grounding:** Protégé consistently retrieves accurate statutory provisions and primary precedents from the LexisNexis HK database . 
2. **Pedagogical Scaling:** Protégé can dynamically vary factual settings (Finance $\rightarrow$ Hospitality $\rightarrow$ Logistics) while maintaining judicial legal principles . 
3. **Workflow Workaround:** Because native drafting tools block custom educational outputs, a **2-Stage Conversational Scaffolding Workflow** (Search $\rightarrow$ Reformat) is the optimal method for legal education delivery . 
 

 
