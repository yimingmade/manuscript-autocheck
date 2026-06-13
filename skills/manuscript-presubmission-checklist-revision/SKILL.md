---
name: manuscript-presubmission-checklist-revision
description: Use when reviewing a manuscript, tables, or supplementary materials before journal submission to systematically check cross-file data consistency, formatting, abbreviations, referencing, and data integrity issues.
---

# Manuscript Pre-Submission Checklist (Revision)

## Overview

You are an experienced, detailed, meticulous researcher conducting a systematic pre-submission check of a manuscript, its tables, and supplementary materials. Work through each category below in order. For each issue found, report: the **category**, the **location** (section, page, line, table, or figure number where identifiable), the **exact text or value**, and the **nature of the problem**. Do not correct issues silently. Flag everything for the author's review.

**Before beginning any checks:** If the document contains tracked changes or comments, ignore them entirely. Perform all checks only on the accepted, final text. Do not flag unresolved tracked changes or comments as issues.

**Report format:** Begin with a summary line stating how many issues were found across how many categories. Then list findings by category in the order below. If a category has no issues, state "No issues found" for that category.

**Detailed reporting requirements:**

- Never condense findings with phrases such as "multiple instances," "multiple lines," "several instances," "various places," or any equivalent grouped wording. The report must be a thorough log of every error found. List each issue fully and systematically so the author can locate and address every one.
- If many findings share the same underlying problem, still report each occurrence separately with its own location, exact observed text or value, expected or correct text/value where determinable, and the reason it is wrong.
- Be specific and detailed in every finding. State what is wrong, what should be correct, and why. When the correct value or text cannot be determined from the supplied files, state: "Correct value/text not determinable from supplied files; author verification required."
- Use comparison tables whenever they make discrepancies easier to verify, especially for Category 0 data consistency, Category 24 response-text accuracy, or any issue involving more than two locations or values.
- Number issues within each category using this structure: "Issue 1 — [specific descriptive title]". For each issue, include the relevant category, location(s), observed value/text, correct or expected value/text, comparison source(s), and author action required.
- Do not silently correct or normalise anything. The output is an audit trail, not an edited manuscript.

**Example of sufficiently detailed reporting for Category 0:**

Issue 1 — Abstract and "Research in Context" vs. Results section: overall decomposition values

The three key percentages in the decomposition analysis differ between the Abstract/Research in Context and the Results section.

| Component | Abstract (line 87) | Research in Context Implications (line 109) | Results section (line 167) |
|---|---:|---:|---:|
| Population growth | 56·9% | 56·9% | 48.5% |
| Population aging | 66·0% | 66·0% | 66·6% |
| Risk exposure | −68·8% | not stated | −89.4% |

The Abstract and Research in Context are internally consistent with each other but differ from the Results section on all three values. One set of figures is incorrect. Flag for author verification.

Issue 2 — Discussion vs. Results section: metabolic risk decomposition values

Both sections discuss the decomposition of crude CVD-related DALYs attributable to metabolic risk factors from 1990 to 2023, but report different figures.

| Location | Exact text/value reported |
|---|---|
| Discussion (line 217) | "population growth and population aging contributing to 73·9% and 53·3% increases in crude DALYs respectively" |
| Results (line 173) | "population growth (63.7%) and population aging (55·4%)" |
| Response to Reviewer 6 Comment 2 | cites the Discussion values, 73·9% and 53·3% |

The response confirms the Discussion values are intentional in that section, but they contradict the Results section. Flag for author verification.

---

## Checklist

### 0. Data Consistency Across All Files *(Highest Priority — Complete Before All Other Checks)*

**Step 1 — Build a complete data inventory.** Before reading the manuscript, read every table and every supplementary file in full. For each file, extract and internally record every numerical value, statistic, and data point along with its label, row/column context, and source location (e.g. "Table 2, row 'Hypertension', column 'HR (95% CI)': 1.47 (1.12–1.93)"). Do not skim. Do not summarise. Read every cell.

**Step 2 — Check the manuscript against the inventory.** Read the manuscript text. For every numerical value, statistic, or data point cited in the manuscript, look it up in the inventory built in Step 1. Verify that:
- The value in the manuscript exactly matches the value in the corresponding table or supplementary file.
- The context is the same (same variable, same subgroup, same timepoint, same model).

Flag every discrepancy. Include: the value as it appears in the manuscript, the value as it appears in the source table or supplementary file, and both locations.

> Example: Manuscript states "the adjusted HR for hypertension was 1.47 (95% CI 1.12–1.93)"; Table 2 shows 1.74 (1.12–1.93). Flag as: **Manuscript vs Table 2 mismatch — HR value: manuscript reports 1.47, table reports 1.74.**

**Do not proceed to checks 1–27 until this step is fully complete.**

---

### 1. Number Formatting: Decimal Places and Significant Figures

Check that all reported numerical values are presented consistently within each statistic type. Group values by type (e.g. adjusted hazard ratios, 95% confidence intervals, p-values, cT1 values, beta coefficients) and verify that all values of the same type are reported to the same number of decimal places or significant figures throughout the manuscript, tables, and supplementary materials. Flag any value within a group that deviates from the most common format used for that group.

> Example: If aHR values are reported as 1.23, 0.87, 1.04 in most places but appear as 1.2 or 1.045 elsewhere, flag those as inconsistent.

---

### 2. Number Formatting: Presentation of Large Numbers

Check that all large numbers use comma separators consistently (e.g. 10,000 not 10000). Flag any large number that is missing comma separators or uses a different convention (e.g. spaces or periods as thousands separators).

---

### 3. Number Formatting: Redundant Zero Expressions

Check for any instance where a value of zero is expressed with redundant repetition, such as "0 (0, 0)", "0 (0–0)", "0 [0, 0]", or similar patterns where a zero value is followed by a parenthetical or bracketed range that is also entirely zero. The correct presentation is simply "0". Flag every such instance with its location.

Do not flag values such as "0.0" when they are part of a larger legitimate non-zero data field or uncertainty interval, such as "50.0 (40.0 to 56.0)" or "50.0 (40.0–56.0)". Only flag redundant zero expressions where the point estimate is zero and the entire accompanying interval/range is also zero or negative-zero, such as "0 (0 to 0)", "0.0 (0.0 to 0.0)", "0 [0, 0]", or "-0 (-0 to 0)".

---

### 4. Order of Figures and Tables

Check that all figures and tables are cited in the manuscript text in numerical order (Figure 1 before Figure 2, Table 1 before Table 2, etc.). Check the same for supplementary figures and supplementary tables. Flag any citation that appears out of sequence.

---

### 5. Figures and Supplementary Materials: Numbering Consistency

Check that every figure, table, supplementary figure, and supplementary table that is numbered in the manuscript is correctly numbered in the supplementary materials file, and vice versa. Flag any mismatch between how an item is labelled in the manuscript text and how it is labelled in the actual figure, table, or supplementary file.

---

### 6. Data Presented Outside the Results Section

Check whether any specific numerical results, effect sizes, statistical values, or data points are presented for the first time outside the Results section (e.g. in the Introduction, Discussion, or Abstract). Flag these for review, as key data should generally be introduced in the Results section before being referenced elsewhere.

---

### 7. Superscript Formatting

Check that all superscripts are correctly formatted, including footnote markers in tables, reference citations, and statistical notation (e.g. cm², m/s²). Flag any superscript that appears to have reverted to regular text, or any regular text that should be superscripted.

---

### 8. Consistent Terminology for the Same Concept

Check for instances where the same clinical, statistical, or methodological concept is referred to using different terms across the manuscript, tables, and supplementary materials. Flag all variant terms and list them together so the author can decide on a single preferred term. Do not standardise without instruction.

> Example: "Cardiovascular-related mortality," "CV-related mortality," and "cardiovascular mortality" may all refer to the same endpoint. Flag these as potentially inconsistent.

---

### 9. Inappropriate Capitalisation

Check for inconsistent or inappropriate capitalisation of clinical terms, study names, intervention names, and statistical terms. Flag words that are capitalised in some places but not others, and words that appear to be incorrectly capitalised (e.g. "Hazard Ratio" vs "hazard ratio," "Cardiovascular Disease" vs "cardiovascular disease"). Do not flag proper nouns, acronyms, or terms that are conventionally capitalised.

---

### 10. Undefined Abbreviations: Main Text

Check that every abbreviation is defined at its first use in the main manuscript text. Flag any abbreviation that appears without a definition at first use.

---

### 11. Undefined Abbreviations: Tables

Check every table independently. Every abbreviation that appears within a table — including column headers, row labels, and cell values — must be defined in a footnote directly beneath that table. It is not sufficient for an abbreviation to have been defined earlier in the main text or in a previous table. Flag any abbreviation in a table that does not have a corresponding footnote definition in the same table.

---

### 12. Undefined Abbreviations: Supplementary Materials

Check that abbreviations used in supplementary figures and supplementary tables are defined in the relevant legend or footnote for that item. Flag any abbreviation that appears without a definition in its immediate supplementary context.

---

### 13. Duplicate References

Check the reference list for duplicate entries, defined as the same source appearing more than once under different reference numbers. Flag the duplicate entries with their reference numbers.

---

### 14. Reference Formatting Consistency

Check that all references in the reference list follow the same formatting convention, including author name format, journal name format (abbreviated or full), punctuation, and the presence or absence of DOIs or URLs. Flag any reference that deviates from the predominant format used in the list.

---

### 15. Unfilled Placeholders

Search the entire document, including tables and supplementary materials, for any unfilled placeholders. These typically appear as "XX," "XXX," "TBC," "INSERT," "[AUTHOR]," or similar. Flag every instance with its location.

---

### 16. Incidence versus Prevalence

Check that "incidence" and "prevalence" are used with their correct epidemiological meanings throughout.

- **Incidence:** the number of new cases of a condition arising in a defined population over a specified time period.
- **Prevalence:** the total proportion of a population with a condition at a given point in time or over a defined period.

Flag any instance where these terms appear to be used interchangeably, incorrectly, or ambiguously.

---

### 17. P-value Bolding

Check all reported p-values throughout the manuscript, tables, and supplementary materials. Flag in both directions:

- Any p-value that is statistically significant (p < 0.05) that is **not** bolded.
- Any p-value that is not statistically significant (p ≥ 0.05) that **is** bolded.

Report the location, the p-value, and which direction the error runs.

---

### 18. Spelling Preference: American or British English

Before checking spelling, determine whether the user has specified a preferred spelling convention for this review:
- If the user specifies American English, flag British English spellings.
- If the user specifies British English, flag American English spellings.
- If the user gives no preference, assume American English is desired and flag British English spellings.

Check for any word whose spelling does not align with the selected convention. Flag each instance with the spelling found, the expected spelling under the selected convention, and the preference applied. Do not correct; flag for author review.

Common examples to check:

| American | British |
|----------|---------|
| analyze | analyse |
| randomized | randomised |
| center | centre |
| fiber | fibre |
| categorize | categorise |
| favor | favour |
| color | colour |
| tumor | tumour |

---

### 19. Data Citation Completeness

When the manuscript text states that data can be found in a specific figure or table (e.g. "as shown in Figure 2"), check whether the same data also appear in other figures, tables, or supplementary items that are not cited at that point. Flag any apparent omissions for the author's consideration.

---

### 20. Supplementary Material Cross-References

Check that all in-text citations of supplementary materials refer to the correct supplementary item number. Flag any cross-reference that appears to point to the wrong supplementary figure, table, or file based on context.

---

### 21. Corresponding Author Details

Check that the corresponding author named in the manuscript matches the corresponding author listed in any cover letter, title page, or submission form included in the documents you have been given. Flag any discrepancy.

---

### 22. Single-Use Abbreviations

Check the main manuscript text, all tables, and all supplementary materials for abbreviations that are defined but used only once. An abbreviation is inappropriate if it is introduced with its full form (e.g. "cardiovascular disease (CVD)") but the abbreviated form then appears only that one time, or not at all thereafter. In such cases, the abbreviation adds no value and the full term should be used throughout instead.

For each instance, report: the abbreviation, the full term it replaces, and the location where it is defined. Flag for the author's consideration whether to remove the abbreviation and use the full term instead.

> Example: "Left ventricular ejection fraction (LVEF) was measured at baseline." If "LVEF" does not appear again in the manuscript, tables, or supplementary materials, flag this as a single-use abbreviation.

---

### 23. Response to Reviewers: Coverage of All Comments

The response to reviewers document contains reviewer comments in **black** text and the author's responses in **red** text (where present).

Check that every reviewer comment in black has a corresponding response in red. Flag any reviewer comment that has no red response, or where the red response appears to be missing, incomplete, or inadvertently left blank.

---

### 24. Response to Reviewers: Accuracy of Cited Text

When a response to a reviewer cites text from another document, such as the manuscript, the Results section, the Methods section, supplementary materials, or supplementary methods, check that the quoted or paraphrased text in the response exactly matches the corresponding text in the source document.

For each such citation in the response to reviewers:
- Locate the cited passage in the relevant source document.
- Compare the text word for word.
- Flag any discrepancy, including differences in wording, values, order, or omission of content.

> Example: If a response states "We have revised the Results section to read: 'The adjusted HR was 1.47 (95% CI 1.12–1.93)'," but the actual manuscript Results section reads "The adjusted HR was 1.74 (95% CI 1.12–1.93)," flag this as a mismatch.

---

### 25. Response to Reviewers: Citation Endnotes Within Each Response

Check that every citation made within the response to reviewers document is supported by an endnote or reference listed within that same response entry. It is not sufficient for a reference to appear only in the main manuscript reference list.

Flag any instance where a source is cited in a response (e.g. as a numbered reference, author-year, or similar) without a corresponding endnote or reference entry in that response.

---

### 26. Response to Reviewers: Application of All Prior Checks

All checks from categories 0–22 above also apply to the response to reviewers document. This includes:

- Data consistency: any numerical values, statistics, or data points in the response must match the corresponding values in the manuscript, tables, and supplementary materials.
- Unfilled placeholders (check 15): flag any "XX," "TBC," "INSERT," or similar in the response document.
- Any other formatting, terminology, or consistency checks where applicable.

Apply these checks to the response to reviewers document as a separate pass after completing checks 0–22 on the main manuscript and supplementary files.

---

### 27. Final Layout Pass: Unnecessary Page Breaks and Spacing

As the final step, inspect the rendered layout and the document structure for the manuscript, tables, supplementary materials, and response-to-reviewers document. Flag, but do not silently correct:

- Manual page breaks or section breaks that create avoidable blank space, blank pages, or isolated short paragraphs.
- Large vertical gaps caused by repeated empty paragraphs, excessive paragraph spacing before/after, excessive line spacing, or keep-with-next/page-break-before settings.
- Tables, figures, captions, headings, reviewer comments, author responses, or reference-list items separated from their related content by avoidable page breaks or spacing.
- Any page where a small formatting adjustment could clearly reduce an unnecessary blank area without harming readability.

For each issue, report the document, page number where identifiable, nearby heading/table/figure/paragraph text, and the apparent cause (e.g. manual page break, blank paragraphs, spacing before/after, section break, keep-with-next).
