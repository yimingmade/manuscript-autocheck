# Manuscript Autocheck Skills

Codex skills for auditing manuscripts, tables, supplementary materials, and response-to-reviewers documents before journal submission.

## Checks At A Glance

The revision skill includes all checks below. The base pre-submission skill includes checks 0 to 22, with its final layout pass as check 23.

🟧 1. **Data Consistency Across All Files** checks that manuscript values match the source tables and supplementary files.

```text
Manuscript: adjusted HR 1.47
Table 2: adjusted HR 1.74
```

🟧 2. **Number Formatting: Decimal Places and Significant Figures** checks that the same statistic type is reported with consistent precision.

```text
aHR values: 1.23, 0.87, 1.2
```

🟧 3. **Number Formatting: Presentation of Large Numbers** checks that large numbers use the same thousands separator style.

```text
Reported as 10000 in one place and 10,000 elsewhere
```

🟧 4. **Number Formatting: Redundant Zero Expressions** flags zero values with unnecessary zero intervals.

```text
0 (0 to 0)
```

🟧 5. **Order of Figures and Tables** checks that figures and tables are cited in numerical order.

```text
Figure 2 cited before Figure 1
```

🟧 6. **Figures and Supplementary Materials: Numbering Consistency** checks that in-text labels match the actual figure, table, or supplementary item labels.

```text
Text cites Supplementary Table 3, file label says Supplementary Table 2
```

🟧 7. **Data Presented Outside the Results Section** flags numerical results introduced first outside the Results section.

```text
Discussion first reports a hazard ratio not stated in Results
```

🟧 8. **Superscript Formatting** checks footnote markers, references, and units that should be superscripted.

```text
cm2 used where cm² is intended
```

🟧 9. **Consistent Terminology for the Same Concept** flags variant terms that appear to describe the same concept.

```text
cardiovascular mortality
CV-related mortality
cardiovascular-related mortality
```

🟧 10. **Inappropriate Capitalisation** checks inconsistent or inappropriate capitalisation of terms.

```text
Hazard Ratio in one section, hazard ratio elsewhere
```

🟧 11. **Undefined Abbreviations: Main Text** checks that abbreviations are defined at first use in the main text.

```text
CVD appears before cardiovascular disease (CVD)
```

🟧 12. **Undefined Abbreviations: Tables** checks that each table defines its own abbreviations in a footnote.

```text
Table header uses aHR, but table footnote does not define aHR
```

🟧 13. **Undefined Abbreviations: Supplementary Materials** checks that supplementary figures and tables define abbreviations in their immediate context.

```text
Supplementary Figure 4 uses BMI without legend definition
```

🟧 14. **Duplicate References** checks whether the same source appears more than once in the reference list.

```text
Reference 12 and Reference 34 describe the same article
```

🟧 15. **Reference Formatting Consistency** checks whether references follow the same author, journal, punctuation, DOI, and URL style.

```text
Most references use abbreviated journal names, one uses the full journal name
```

🟧 16. **Unfilled Placeholders** searches for unresolved placeholders across manuscript files.

```text
INSERT TABLE TITLE
```

🟧 17. **Incidence versus Prevalence** checks whether these epidemiological terms are used with their correct meanings.

```text
Prevalence described as new cases per year
```

🟧 18. **P-value Bolding** checks whether significant and non-significant p-values are bolded appropriately.

```text
p=0.032 not bolded
p=0.18 bolded
```

🟧 19. **Spelling Preference: American or British English** checks spelling against the user-specified convention, defaulting to American English if no preference is given.

```text
Preference: American English
Found: randomised
Expected: randomized
```

🟧 20. **Data Citation Completeness** checks whether a statement cites all relevant figures, tables, or supplementary items containing the same data.

```text
Text cites Figure 2 only, but the same subgroup data also appear in Supplementary Table 5
```

🟧 21. **Supplementary Material Cross-References** checks that supplementary citations point to the correct item.

```text
Text cites Supplementary Figure 1 for baseline characteristics, but those data are in Supplementary Table 1
```

🟧 22. **Corresponding Author Details** checks corresponding author details across manuscript, cover letter, title page, and submission forms.

```text
Title page lists Author A, cover letter lists Author B
```

🟧 23. **Single-Use Abbreviations** checks for abbreviations that are defined but used only once.

```text
left ventricular ejection fraction (LVEF), with no later LVEF use
```

🟧 24. **Response to Reviewers: Coverage of All Comments** checks that every reviewer comment has an author response.

```text
Reviewer 2 Comment 4 has no red response text
```

🟧 25. **Response to Reviewers: Accuracy of Cited Text** checks that quoted or paraphrased response text matches the source document.

```text
Response says HR 1.47
Revised manuscript says HR 1.74
```

🟧 26. **Response to Reviewers: Citation Endnotes Within Each Response** checks that citations in each response are supported within that same response entry.

```text
Response cites reference 6, but no endnote or reference appears in that response
```

🟧 27. **Response to Reviewers: Application of All Prior Checks** applies checks 0 to 22 to the response-to-reviewers document.

```text
Response contains TBC in a revised-methods explanation
```

🟧 28. **Final Layout Pass: Unnecessary Page Breaks and Spacing** checks rendered documents for avoidable blank space, page breaks, and separated captions or responses.

```text
Manual page break leaves a half-empty page before Table 1
```

## Contents

- `skills/manuscript-presubmission-checklist/SKILL.md` - pre-submission checklist for manuscripts, tables, and supplementary materials.
- `skills/manuscript-presubmission-checklist/agents/openai.yaml` - optional Codex UI metadata.
- `skills/manuscript-presubmission-checklist-revision/SKILL.md` - revision-stage checklist for manuscripts, supplementary materials, and response-to-reviewers documents.
- `skills/manuscript-presubmission-checklist-revision/agents/openai.yaml` - optional Codex UI metadata.

## Install

Install both skills from this repository:

```bash
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist skills/manuscript-presubmission-checklist-revision
```

Or install one skill at a time:

```bash
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist-revision
```

Or copy the skill directories directly:

```bash
cp -R skills/manuscript-presubmission-checklist ~/.codex/skills/
cp -R skills/manuscript-presubmission-checklist-revision ~/.codex/skills/
```

Restart Codex after installation.

## Dependencies

The skill has no local file, script, package, or runtime dependencies.

## Licence

MIT License. See `LICENSE`.
