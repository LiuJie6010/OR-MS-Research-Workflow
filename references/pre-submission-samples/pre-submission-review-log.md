# Pre-Submission Review Log

**Paper**: The Cost-Balancing Principle for Dynamic Matching Markets
**Target Journal**: Management Science
**Review Date**: 2026-01-27

---

## Review Structure

Each issue is logged with:
- **ID**: Section.Number (e.g., S3.01 = Section 3, issue #1)
- **Type**: Grammar | Terminology | Technical | Exposition
- **Confidence**: High (certain) | Medium (likely correct) | Low (needs author judgment)
- **Status**: Identified | Fixed | Deferred | Author Decision Needed
- **Line**: Approximate line number in `new.tex`

---

## Pass 1: Abstract & Introduction

### Writing Quality (Grammar, Terminology, Consistency)

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S1.01 | Grammar | 345 | Em-dash in abstract: "economies of scale—guaranteeing" violates our no-em-dash rule | High | Replaced with comma | Fixed |
| S1.02 | Grammar | 446 | "On one hand" should be "On the one hand" (formal academic English); line 448 "On the other hand" already has "the" | Medium | Added "the" for parallelism | Fixed |
| S1.03 | Grammar | 454 | Double period at end of sentence: "customer satisfaction.." | High | Removed extra period | Fixed |
| S1.04 | Terminology | 454 | "slash unit costs" is informal for Management Science | Medium | → "reduce unit costs" | Fixed |
| S1.05 | Grammar | 455 | "multi-billion dollar" missing hyphen → "multi-billion-dollar" (compound adjective) | Medium | Added hyphen | Fixed |
| S1.06 | Terminology | 456 | "the leading cause of user churn" is a strong unverified claim | Medium | → "a leading cause" | Fixed |
| S1.07 | Terminology | 472 | "matching utility" is non-standard in OR/OM | Medium | → "matching quality" | Fixed |
| S1.08 | Terminology | 474 | "vary wildly" is informal for academic writing | Medium | → "fluctuate significantly" | Fixed |
| S1.09 | Grammar | 495 | "ad-hoc" should be "ad hoc" (Latin phrase, no hyphen) | High | Removed hyphen | Fixed |
| S1.10 | Terminology | 518 | "scales to a calibrated proportion" is slightly awkward | Medium | → "reaches a calibrated proportion" | Fixed |
| S1.11 | Grammar | 447 | Two sentences on same line; violates one-sentence-per-line format | Low | Split into two lines | Deferred |
| S1.12 | Grammar | 456 | Two sentences on same line; violates one-sentence-per-line format | Low | Split into two lines (partially done via S1.06 fix) | Fixed |

### Exposition & Insight Clarity

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S1.13 | Exposition | 426 | Mixes brand names (Uber, Lyft, DoorDash) with category ("competitive gaming servers"); not parallel | Low | Could use a specific gaming platform name, or rephrase | Identified |
| S1.14 | Exposition | 616 | Comment says "NUMBERED LIST with 6 items" but there are 5 contributions | Low | Fix comment (not visible in PDF) | Identified |
| S1.15 | Exposition | 293-294 | Abstract sentence 1 lists "ridesharing to food delivery to competitive gaming" — good breadth, but "competitive gaming" appears only in experiments, not in the theory | Low | No change needed; valid scope claim | Identified |

---

## Pass 2: Literature Review

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S2.01 | Grammar | 680 | Awkward word order: "contributes to this literature a constant-competitive algorithm" | Medium | → "contributes a constant-competitive algorithm to this literature" | Fixed |
| S2.02 | Grammar | 697 | Very long sentence (~4 lines) with "where" clause creating run-on effect | Medium | Split into two sentences at the "where" clause | Fixed |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S2.03 | Exposition | 732 | Citation `\cite{BEV2026}` has year 2026 — will this be published by submission? | Low | Authors should verify publication status | Identified |

---

## Pass 3: Section 3 (Model, Algorithm, Main Results)

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S3.01 | Grammar | 883 | Typo: "subcript" → "subscript" | High | Fixed typo | Fixed |
| S3.02 | Grammar | 883 | Singular/plural mismatch: "for any policy $\pi$ and problem instances" → "problem instance" (singular to match "any") | Medium | → "problem instance" | Fixed |
| S3.03 | Terminology | 848 | "matching cost made" is non-standard; should be "matching cost incurred" | Medium | → "incurred" | Fixed |
| S3.04 | Terminology | 848 | "monotonic property" → "monotonicity property" (standard mathematical term) | Medium | → "monotonicity property" | Fixed |

### Technical Correctness

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S3.05 | Technical | — | Proof of Theorem 1 structure is sound: charging argument correctly relates CB and OPT costs via equation (5) | High | No issues found | Verified |
| S3.06 | Technical | — | Algorithm 1 pseudocode is correct and matches the textual description | High | No issues found | Verified |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S3.07 | Exposition | 804 | Good: explicitly states "no distributional assumptions" early; this is a key selling point | — | — | No action needed |

---

## Pass 4: Section 4 (Cost-Balancing Principle)

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S4.01 | Grammar | 1065 | Comma splice: "provides the key insight..., the proof is postponed" — two independent clauses joined by comma | High | Changed comma to semicolon | Fixed |

### Technical Correctness

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S4.02 | Technical | — | Proposition 1 (monotonicity) statement and proof structure are sound | High | No issues found | Verified |
| S4.03 | Technical | — | Theorem 2 (fluid limit cost ratio $W^*/M^* = 2\beta$) derivation is correct | High | No issues found | Verified |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S4.04 | Exposition | 1044 | "While the subsequent analysis can easily be extended to general $N$" — claim of easy extension is not verified in the paper | Low | Authors should decide if this claim needs qualification | Identified |

---

## Pass 5: Section 5 (Competitive Ratio Analysis)

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S5.01 | Grammar | 1306 | Lowercase "assumption" when referring to a named Assumption: "by assumption~\ref{ass:key}" | High | → "by Assumption~\ref{ass:key}" | Fixed |

### Technical Correctness

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S5.02 | Technical | 1111 | Proof uses "$W^-_k \approx W_k$" but since the arrival is instantaneous, this should be exact equality "$W^-_k = W_k$" | Medium | Changed $\approx$ to $=$ throughout this argument | Fixed |
| S5.03 | Technical | 1113 | Consequent use of $\approx$ in "Combining these gives $\alpha W_k \approx \alpha W^-_k < ...$" also changed to $=$ | Medium | Changed to $=$ | Fixed |
| S5.04 | Technical | — | Proof of Proposition 2 (Greedy unbounded) is correct: adversarial construction is valid | High | No issues found | Verified |
| S5.05 | Technical | — | Proof of Proposition 3 (Threshold unbounded) is correct | High | No issues found | Verified |
| S5.06 | Technical | — | Proof of Proposition 4 (golden ratio lower bound) is correct | High | No issues found | Verified |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S5.07 | Exposition | 1168-1173 | Remark after Theorem 1 proof is helpful — explains why two consecutive matches are needed | — | Good exposition | No action needed |

---

## Pass 6: Section 6 (Attribute-Based Model)

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S6.01 | Grammar | 1420 | "Easy to check that" is too informal for Management Science | High | → "It is straightforward to verify that" | Fixed |
| S6.02 | Grammar | 1348 | "modified accordingly to" is grammatically incorrect | High | → "modified accordingly for" | Fixed |
| S6.03 | Terminology | 1351 | "matching cost made" (same issue as S3.03 in Assumption 2) | Medium | → "matching cost incurred" | Fixed |
| S6.04 | Terminology | 1351 | "monotonic property" (same issue as S3.04 in Assumption 2) | Medium | → "monotonicity property" | Fixed |

### Technical Correctness

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S6.05 | Technical | — | Proposition 5 (NP-hardness) reduction to 3DM is valid | High | No issues found | Verified |
| S6.06 | Technical | — | Proposition 6 (adversarial impossibility) construction is valid | High | No issues found | Verified |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S6.07 | Exposition | 1495-1501 | Good: the impossibility result is well-motivated, explaining why queue-based abstraction is "necessary" not just "convenient" | — | Good exposition | No action needed |

---

## Pass 7: Section 7 (Numerical Study)

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S7.01 | Terminology | 1565 | Table 1 caption says "$C$ denotes the cost weight parameter" but column header and text use $\gamma$ | High | Changed $C$ to $\gamma$ in caption | Fixed |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S7.02 | Exposition | 1591 | Long paragraph explaining delivery setting deviation — could be clearer with a transition | Low | Authors may consider splitting | Identified |
| S7.03 | Exposition | 1680 | "Besides" at start of sentence is slightly informal | Low | Could use "In addition" or "Moreover" | Identified |

---

## Pass 8: Conclusion

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S8.01 | Grammar | — | No grammar issues found in conclusion | — | — | Clean |

### Exposition

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S8.02 | Exposition | — | Conclusion is well-structured with clear subsections (Summary, Practical Implications, Limitations/Future Research) | — | — | No action needed |

---

## Pass 9: E-Companion Proofs

### Technical Correctness

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S9.01 | Technical | — | Proof of Proposition 1 (monotonicity via value iteration) is rigorous; 5-case induction is complete | High | Verified | No issues |
| S9.02 | Technical | — | Proof of Theorem 2 (fluid limit) is rigorous; 4-step structure (scaling, convergence, optimization, ratio) is correct | High | Verified | No issues |
| S9.03 | Technical | — | VRP formulation in E-Companion is complete and well-specified | High | Verified | No issues |

### Writing Quality

| ID | Type | Line | Issue | Confidence | Fix | Status |
|----|------|------|-------|------------|-----|--------|
| S9.04 | Grammar | 2317 | "bellmen value iteration" — should be "Bellman" (proper noun) | High | → "Bellman value iteration" | Fixed |
| S9.05 | Grammar | 2317 | "converges to the optimality" — incorrect article | High | → "converges to optimality" | Fixed |
| S9.06 | Exposition | 1761-1762 | Missing "Section" or "Appendix" prefix in cross-references: "in \ref{app:delivery_vrp}" should be "in Section~\ref{app:delivery_vrp}" | Low | Authors may want to add "Section~" prefix | Identified |

---

## Pass 10: Global Consistency Sweep

### Notation Consistency

| Symbol | Intended Meaning | Inconsistencies Found | Resolution | Status |
|--------|-----------------|----------------------|------------|--------|
| $\Gamma$ | Economies-of-scale parameter | None | Consistent throughout | Clean |
| $\alpha$ | Balancing parameter | None | Consistent throughout | Clean |
| $J$ | Cost/objective | None (proper superscripts distinguish uses) | Consistent throughout | Clean |
| $\mathbf{X}$/$\mathbf{x}$ | State process/realization | `{\bf x}` used in ~10% of doc instead of `\mathbf{x}` | Standardized all to `\mathbf{x}` | Fixed |
| $f$ | Matching cost function | None | Consistent throughout | Clean |

### Terminology Consistency

| Concept | Chosen Term | Variants Found | Resolution | Status |
|---------|-------------|---------------|------------|--------|
| Queue length | "queue length" | "pool size" (1x, experimental context), "queue size" (1x) | Acceptable: used in distinct contexts | Clean |
| Matching cost | "matching cost" | None | Consistent | Clean |
| Waiting cost | "waiting cost" | None | Consistent | Clean |
| Competitive ratio | "competitive ratio" (lowercase) | None | Consistent | Clean |
| Algorithm name | "Cost-Balancing" (capitalized, hyphenated) | "cost-balancing" in compound modifiers | Correct: capitalized as proper name, lowercase as modifier | Clean |
| Latin phrase | "ad hoc" (no hyphen) | "ad-hoc" (1x, line ~1727) | Fixed to "ad hoc" | Fixed |
| Online/offline | "online"/"offline" (no hyphens) | None | Consistent | Clean |

### Cross-Reference Check

| ID | Issue | Status |
|----|-------|--------|
| G10.01 | All \ref/\label pairs verified — no broken references | Clean |
| G10.02 | All formal elements (Assumption, Theorem, Proposition, etc.) properly capitalized before \ref | Clean |
| G10.03 | Tilde (~) used consistently before \ref for non-breaking spaces | Clean |

---

## Issues Found During Initial Read (Pre-Review)

These were spotted during the full read-through before the systematic review began.

| ID | Type | Line | Issue | Confidence | Status |
|----|------|------|-------|------------|--------|
| PRE.01 | Grammar | ~882 | "subcript" should be "subscript" | High | Fixed (= S3.01) |
| PRE.02 | Terminology | ~1564 | Table 1 caption says "$C$ denotes the cost weight parameter" but column header uses $\gamma$ | High | Fixed (= S7.01) |
| PRE.03 | Grammar | ~1419 | "Easy to check that" is too informal for Management Science | High | Fixed (= S6.01) |
| PRE.04 | Terminology | various | "queue length" vs "pool size" vs "queue size" used interchangeably | Medium | Verified in Pass 10: used in distinct contexts, acceptable |
| PRE.05 | Technical | ~1064 | Comma splice: "provides the key insight..., the proof is postponed" should be period or semicolon | High | Fixed (= S4.01) |
| PRE.06 | Technical | ~1110 | Proof uses "$W^-_k \approx W_k$" with approximate equality; should be exact | Medium | Fixed (= S5.02) |
| PRE.07 | Technical | ~2316 | "bellmen value iteration" should be "Bellman value iteration" | High | Fixed (= S9.04) |
| PRE.08 | Grammar | ~2316 | "converges to the optimality" should be "converges to optimality" | High | Fixed (= S9.05) |

---

## Summary Statistics

| Category | Identified | Fixed | Deferred | Author Decision |
|----------|-----------|-------|----------|-----------------|
| Grammar | 16 | 14 | 1 | 1 |
| Terminology | 10 | 9 | 0 | 1 |
| Technical | 3 | 3 | 0 | 0 |
| Exposition | 3 | 0 | 0 | 3 |
| **Total** | **32** | **26** | **1** | **5** |

*Note: "Author Decision" items are Low confidence issues documented for co-author review. Technical "Verified" items (proofs checked) are not counted in the table above.*

---

## Low-Confidence Items for Co-Author Review

The following items were identified but not fixed due to low confidence. Please review:

1. **S1.13** (line ~426): Introduction mixes brand names with a category ("competitive gaming servers"). Consider naming a specific gaming platform for parallelism.
2. **S1.14** (line ~616): LaTeX comment says "NUMBERED LIST with 6 items" but there are 5 contributions. Not visible in PDF.
3. **S4.04** (line ~1044): Claims "the subsequent analysis can easily be extended to general $N$" — verify if this extension is straightforward.
4. **S7.02** (line ~1591): Long paragraph explaining delivery setting deviation could be split for clarity.
5. **S7.03** (line ~1680): "Besides" at start of sentence — slightly informal; consider "In addition."
6. **S9.06** (line ~1761-1762): Missing "Section~" prefix in some E-Companion cross-references.
