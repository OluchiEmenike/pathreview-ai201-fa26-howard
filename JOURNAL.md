## Unit 7 — Issue selection

**Issue link:** [[paste link here](https://github.com/codepath/pathreview-ai201-fa26-howard/issues/11)]

**Issue title:** [Architecture doc doesn't explain the hybrid retrieval scoring formula]

**Tier:** [/] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
The architecture guide says PathReview combines vector search and keyword search, but it doesn’t explain how those results are scored together. In rag/retriever/hybrid.py, each set of scores is normalized and then blended using default weights of 70% vector and 30% keyword. I’ll update docs/ARCHITECTURE.md with the formula and a simple example so contributors can understand how the final ranking is calculated.

**Branch name:** docs/11-hybrid-scoring-formula

**Setup confirmation:** The app successfully runs locally at localhost:5173

**Cohort ledger:** [/] Issue added to cohort ledger