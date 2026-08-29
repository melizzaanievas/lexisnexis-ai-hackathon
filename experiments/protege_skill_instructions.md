# LexisNexis Protégé: Custom Skill & Vault Integration Guide

> **Project:** Protégé Scenario-to-Authority Educational Engine  
> **Skill Name:** `Generate Template Responses`  
> **Vault Document:** `universal_clinic_template_framework.txt`  

---

## 🛠️ Step-by-Step Workflow in LexisNexis Protégé

### **Step 1: Upload Vault Document**
1. Log in to **LexisNexis Protégé**.
2. Navigate to **Vault** $\rightarrow$ **Upload Document**.
3. Upload `universal_clinic_template_framework.txt` into the Vault.

### **Step 2: Activate Skill**
1. Navigate to **Skills** $\rightarrow$ **Custom Skills**.
2. Select or activate the **Generate Template Responses** skill.
3. Ensure the skill is linked to the Vault context containing `universal_clinic_template_framework.txt`.

---

## 🧪 Step 3: Prompt Execution Examples

### **Example A: Personal Data Privacy (Healthcare / Taylor)**
```text
Using universal_clinic_template_framework.txt in my Vault, generate a clinic display card for: 
• [PRIMARY_STATUTE_OR_LAW]: Personal Data (Privacy) Ordinance (Cap. 486) Data Protection Principles 
• [PRIMARY_PRECEDENT]: Relevant HK PCPD guidance & Privacy Commissioner Rulings 
• [INDUSTRY]: Healthcare | [ROLE]: Medical Records Officer | [WORKER_OR_PARTY_NAME]: Taylor 
• [INCIDENT_ACTION_OR_BREACH]: accidentally emailed an unencrypted patient list to an external vendor 
• [HIGH_THRESHOLD_VIOLATION]: Material Data Breach | [LOW_THRESHOLD_DEFENSE]: Inadvertent Administrative Error
```

### **Example B: Employment Summary Dismissal (Finance / Alex)
```text
Using universal_clinic_template_framework.txt in my Vault, generate a clinic display card for:
• [PRIMARY_STATUTE_OR_LAW]: Employment Ordinance (Cap. 57) Section 9(1)(a)(ii)
• [PRIMARY_PRECEDENT]: Tsang Tak Chi v China Wall Ltd [1999] 1 HKC 366
• [INDUSTRY]: Finance | [ROLE]: Financial Analyst | [WORKER_OR_PARTY_NAME]: Alex
• [INCIDENT_ACTION_OR_BREACH]: backed up 50GB of personal family photos to enterprise cloud storage
• [LEGAL_CONSEQUENCE_OR_DISMISSAL]: immediate summary dismissal without notice
• [HIGH_THRESHOLD_VIOLATION]: Gross Misconduct | [LOW_THRESHOLD_DEFENSE]: Minor Negligence
```

### **Example C: Sale of Goods (Retail / Commercial Kitchen)
```text
Using universal_clinic_template_framework.txt in my Vault, generate a clinic display card for:
• [PRIMARY_STATUTE_OR_LAW]: Sale of Goods Ordinance (Cap. 26) Section 12(1)
• [PRIMARY_PRECEDENT]: Relevant HK Commercial Law Precedents on Fitness for Purpose
• [INDUSTRY]: Commercial Catering | [ROLE]: Kitchen Owner | [WORKER_OR_PARTY_NAME]: Commercial Kitchen
• [INCIDENT_ACTION_OR_BREACH]: purchased an industrial oven that fails to reach specified cooking temperatures
• [HIGH_THRESHOLD_VIOLATION]: Repudiatory Breach of Condition | [LOW_THRESHOLD_DEFENSE]: Non-Repudiatory Breach of Warranty
```
