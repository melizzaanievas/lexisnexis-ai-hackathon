# Experiment Log: Dashboard Export to Google Slides, PDF & Presentation Formats

> **Project:** Protégé Scenario-to-Authority Educational Engine  
> **Target Feature:** Multi-Audience Stakeholder Export (Google Slides, PPTX, PDF)  
> **Testing Date:** August 2026  

---

## 🔬 1. Objective

Enable university clinic supervisors, law students, and legal advisors to export live Protégé scenario display cards from the HTML dashboard into presentation formats (Google Slides, PowerPoint, PDF) for executive briefings and client presentations.

---

## 🛠️ 2. Export Architecture

```text
 ┌────────────────────────────────────────────────────────┐
 │           Protégé Live HTML Web Dashboard              │
 └─────────────┬──────────────────────────┬───────────────┘
               │                          │
               ▼                          ▼
 ┌───────────────────────────┐  ┌───────────────────────────┐
 │ 🖨️ One-Click CSS Print    │  │ 📋 Google Slides Copy     │
 │ Engine (Browser to PDF)   │  │ Clipboard Engine (JS)     │
 └─────────────┬─────────────┘  └─────────────┬─────────────┘
               │                          │
               ▼                          ▼
 ┌───────────────────────────┐  ┌───────────────────────────┐
 │ PDF Slide Import into     │  │ Paste Directly into       │
 │ Google Slides / PPTX      │  │ Presentation Decks        │
 └───────────────────────────┘  └───────────────────────────┘
```

---

## 📊 3. Key Implementation Features (index.html) Print Stylesheet (@media print): Strips browser controls, text input boxes, and dropdown menus during printing, preserving clean visual hierarchy.

One-Click Slide Outline Clipboard: Formats scenario cards into structured slide titles and bullet points (**SLIDE** 1, **SLIDE** 2, **SLIDE** 3) ready for Google Slides ingestion.

Multi-Audience Support: Allows exporting both the University Legal Clinic View (for academic/court settings) and the Non-Lawyer Client Takeaway View (for executive/board briefings).

---

