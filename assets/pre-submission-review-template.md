# Pre-Submission Review Template

Use this template for a full-paper pre-submission audit. Fill only statuses that were actually checked.

```markdown
# Pre-Submission Review Log

**Paper**: [Title]
**Target Journal**: [Journal]
**Review Date**: [Date]
**Manuscript Files Inspected**: [Files or extracted text]
**Line Numbers**: [Exact / approximate / unavailable]

---

## Review Structure

Each issue is logged with:
- **ID**: Section.Number, e.g., S3.01 for Section 3 issue 1, G10.01 for global sweep issue 1.
- **Type**: Grammar | Terminology | Technical | Exposition | Notation | Cross-reference | Citation | Table/Figure | Experiment
- **Confidence**: High | Medium | Low
- **Status**: Identified | Fixed | Deferred | Author Decision Needed | Verified | Clean | No action needed
- **Line**: Exact or approximate line number when available.

Status discipline:
- Use **Verified** only after checking the relevant proof, algorithm, equation, experiment, or reference in substance.
- Use **Clean** only after completing the stated sweep and finding no issue.
- Use **Author Decision Needed** for low-confidence style, framing, or scope judgments.

---

## Pass 0: Initial Read

| ID | Type | Location | Issue | Confidence | Recommended Fix or Resolution | Status |
|----|------|----------|-------|------------|-------------------------------|--------|
| PRE.01 | [Type] | [Line/section] | [Issue spotted before systematic pass] | [High/Medium/Low] | [Fix or later ID] | [Status] |

---

## Pass 1: Abstract and Introduction

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix or Recommendation | Status |
|----|------|------|-------|------------|-----------------------|--------|

### Technical Correctness and Claim Calibration

| ID | Type | Line | Issue or Verified Check | Confidence | Fix or Evidence Checked | Status |
|----|------|------|-------------------------|------------|-------------------------|--------|

### Exposition and Framing

| ID | Type | Line | Issue or Positive Check | Confidence | Fix or Recommendation | Status |
|----|------|------|-------------------------|------------|-----------------------|--------|

---

## Pass [N]: [Section Name]

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix or Recommendation | Status |
|----|------|------|-------|------------|-----------------------|--------|

### Technical Correctness

| ID | Type | Line | Issue or Verified Check | Confidence | Fix or Evidence Checked | Status |
|----|------|------|-------------------------|------------|-------------------------|--------|

### Exposition

| ID | Type | Line | Issue or Positive Check | Confidence | Fix or Recommendation | Status |
|----|------|------|-------------------------|------------|-----------------------|--------|

---

## Global Consistency Sweep

### Notation Consistency

| Symbol | Intended Meaning | Inconsistencies Found | Resolution | Status |
|--------|------------------|-----------------------|------------|--------|

### Terminology Consistency

| Concept | Chosen Term | Variants Found | Resolution | Status |
|---------|-------------|----------------|------------|--------|

### Cross-Reference, Citation, Table, and Figure Check

| ID | Issue or Check | Evidence Inspected | Status |
|----|----------------|--------------------|--------|

---

## Issues Found During Initial Read

| ID | Type | Location | Issue | Confidence | Final Status |
|----|------|----------|-------|------------|--------------|

---

## Summary Statistics

| Category | Identified | Fixed | Deferred | Author Decision Needed |
|----------|------------|-------|----------|------------------------|
| Grammar | 0 | 0 | 0 | 0 |
| Terminology | 0 | 0 | 0 | 0 |
| Technical | 0 | 0 | 0 | 0 |
| Exposition | 0 | 0 | 0 | 0 |
| Notation | 0 | 0 | 0 | 0 |
| Cross-reference | 0 | 0 | 0 | 0 |
| Table/Figure | 0 | 0 | 0 | 0 |
| Experiment | 0 | 0 | 0 | 0 |
| **Total** | **0** | **0** | **0** | **0** |

Note: Positive `Verified`, `Clean`, and `No action needed` entries are not counted as fixed issues unless they required a correction.

---

## Low-Confidence Items for Co-Author Review

1. **[ID]** ([location]): [Issue and why author judgment is needed.]

---

## Checks Not Guaranteed

- [List missing files, unavailable line numbers, uninspected appendix sections, unrun experiments, or unresolved dependencies.]
```
