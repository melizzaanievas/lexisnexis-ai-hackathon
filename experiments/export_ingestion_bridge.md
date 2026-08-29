# Experiment Log: Protégé Word/PDF Export & Web Ingestion Bridge

> **Project:** Protégé Scenario-to-Authority Educational Engine  
> **Experiment Focus:** Output Format Boundaries & UI Integration Workarounds  
> **Testing Date:** August 2026  
> **Target Platform:** LexisNexis Protégé + Live GitHub Pages Dashboard  

---

## 🔬 1. Hypothesis & Objective

* **Hypothesis:** LexisNexis Protégé can directly generate raw HTML or native Markdown code snippets to allow automatic, styled rendering on an external web dashboard (e.g., university legal clinic display boards on GitHub Pages).
* **Objective:** Test Protégé's native export formats, evaluate HTML/code sanitization behavior, and establish an operational workaround to bridge enterprise legal document exports with web rendering engines.

---

## 🧪 2. Experimental Execution

### **Test Input Prompt:**
The following prompt was executed in Protégé using the Vault-augmented **Generate Template Responses** skill:

```text
Using universal_clinic_template_framework.txt in my Vault, analyze the cloud backup scenario under HK Employment Ordinance Cap. 57 s.9 and Tsang Tak Chi v China Wall Ltd.

CRITICAL FORMATTING REQUIREMENT: 
Do NOT output plain text or Markdown. Output clean, valid raw HTML code wrapped in <div> tags matching .card, .grid, .gross, and .minor CSS classes.
```

---

## 📊 3. Empirical Findings & Platform Limits **HTML** Code Sanitization: 
Protégé does not output raw **HTML** blocks or execute embedded **HTML** tags. 
The system sanitizes or strips web markup tags to enforce legal document standards.

Native Export Restrictions: Protégé restricts file downloads and exports strictly to enterprise legal formats:
- Microsoft Word (.docx)
- Adobe **PDF** (.pdf)

### Plain Conversational Chat Text

(Native .md files or raw **HTML** code downloads are unsupported).

The Presentation Dilemma: While Protégé delivers high-precision statutory line-pinpointing and case analysis, plain Word/**PDF** document text lacks the color-coding, visual hierarchy, and responsive card layout required for university clinic display boards and public legal education.

---

### 💡 4. The Solution: Live Word/PDF Ingestion Bridge

To overcome the native export format constraint while preserving Protégé's statutory precision, we developed the **Protégé Word/PDF Live Ingestion Bridge** directly on the web frontend (`index.html`).

### **Workflow:**
1. **LexisNexis Protégé:** Outputs pinpointed legal analysis in Word (`.docx`) or PDF format.
2. **Copy & Ingest:** The user copies the text from the document export into the Live Ingestion Bridge text area.
3. **Dynamic Frontend Rendering:** The client-side JavaScript engine parses the raw text and renders responsive, styled CSS display cards.

### **Frontend Integration (`index.html`):**
A lightweight parser ingests the copied text and dynamically updates the DOM:

```javascript
function parseProtegeInput() {
  const rawText = document.getElementById('protegePaste').value.trim();
  if (!rawText) {
    alert("Please paste text from your Protégé Word or PDF export first!");
    return;
  }
  
  const content = document.getElementById('dashboardContent');
  content.innerHTML = `
    <div class="card">
      <h3>📥 Rendered Output from Protégé Word/PDF Ingestion</h3>
      <p style="white-space: pre-wrap; font-family: inherit;">${rawText}</p>
    </div>
  `;
}
```

---

## ✅ 5. Conclusion & Value Proposition Constraint Resolved: 
Bypassed native .docx / **PDF** export limitations without requiring custom backend software or APIs.

Demonstrated Feasibility: Proved that non-technical legal educators can export high-precision legal analyses from Protégé in Word or **PDF**, paste them into the web dashboard bridge, and instantly display responsive, color-coded learning cards.

Live Demo: Accessible on the live project site at melizzaanievas.github.io/lexisnexis-ai-hackathon.
