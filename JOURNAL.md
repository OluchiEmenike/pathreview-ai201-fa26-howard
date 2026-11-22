## Unit 7 — Issue selection

**Issue link:** [[paste link here](https://github.com/codepath/pathreview-ai201-fa26-howard/issues/11)]

**Issue title:** [Architecture doc doesn't explain the hybrid retrieval scoring formula]

**Tier:** [/] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
The architecture guide says PathReview combines vector search and keyword search, but it doesn’t explain how those results are scored together. In rag/retriever/hybrid.py, each set of scores is normalized and then blended using default weights of 70% vector and 30% keyword. I’ll update docs/ARCHITECTURE.md with the formula and a simple example so contributors can understand how the final ranking is calculated.

**Branch name:** docs/11-hybrid-scoring-formula

**Setup confirmation:** The app successfully runs locally at localhost:5173

**Cohort ledger:** [/] Issue added to cohort ledger

**Selection Reasoning**

I chose this issue because this course is my introduction to contributing to a larger codebase, and this Tier 1, good-first-issue task feels like a manageable place to practice. I read the relevant retrieval code and understand that the work is to document the existing scoring formula, default weights, and an example in `docs/ARCHITECTURE.md`, It is done when contributors can follow how the two scores are normalized and blended. The issue estimates 2–3 hours, has no stated blockers, and the change is documentation-only, so I do not expect to need code or test changes. I reviewed the issue comments and claimed it. I still need to check the cohort ledger's Claims count.

## Unit 8 — Reproduction & solution planning

**Reproduction commit link:** [add link after committing this reproduction note]

**Reproduction summary:**
I compared the hybrid retrieval description in `docs/ARCHITECTURE.md` with `HybridRetriever` in `rag/retriever/hybrid.py`. The guide mentions vector and keyword search but omits the score normalization, default weights, and blending formula that the code uses.

**PLAN.md link:** [PLAN.md](./PLAN.md)

**Walkthrough video (recommended):** Not recorded

**Blockers or open questions:** None identified