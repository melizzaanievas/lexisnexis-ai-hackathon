# Standardized Conversational Prompt Templates
> **Jurisdiction:** Hong Kong SAR Employment Law (Cap. 57)

## Template 1: Primary Search & Grounding Prompt (Ask Module)
```text
An employee at a Hong Kong [Industry Type] firm [describe action/incident]. The employer terminated them on the spot without notice or payment in lieu. Under Section [Section Number] of the Hong Kong Employment Ordinance (Cap. 57) and relevant HK case precedents, analyze whether this satisfies the legal threshold for summary dismissal. Direct legal authorities required.

## Template 2: Educational Scaffolding & Display Card Prompt (Ask Module)
```text
Take your legal analysis above and reformat it for a university legal clinic display board. Generate:
1. The Scenario Card: A 3-sentence plain-English story describing a fictional worker named Alex who [describe action] and got fired.
2. The Verdict: A 2-bullet summary explaining if this breach is 'Gross Misconduct' or just 'Minor Negligence' under [Primary Retrieved Precedent].
3. Clinical Exercise: 2 quick true/false questions testing key statutory principles for law students.
