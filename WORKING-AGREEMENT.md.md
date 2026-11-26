# Working agreement: scope, production, and releases

Established: 26 November 2026.

## Purpose

Spend more time producing useful improvements and less time repeatedly uploading, packaging, and correcting the same work. Production is the first priority. Publishing remains an important second priority, not an optional afterthought.

## Adopted rules

### 1. Define scope before starting

At the beginning of each working day/session, restate the scope of the composed component being built, rather than treating each foundation as the whole project.

Record briefly:
- Purpose: the experience we are delivering.
- Included: the work and directly connected elements covered today.
- Excluded: related work we are not undertaking.
- Completion checks: what must work before this scope is done.

Directly connected work may belong inside scope. For example, quick add and the variant-choice popup it needs can belong to the same component work. Do not chase unrelated improvements; record them in a backlog.

### 2. Batch meaningful improvements

Do not consider a normal GitHub upload/release until at least ten meaningful improvements have accumulated.

Ten is the minimum eligibility threshold, not an instruction to publish immediately. Do not count trivial edits or split an outcome artificially to reach ten. The precise counting definition remains subject to agreement; see the proposed refinements below.

### 3. Freeze the release batch

Once we choose a batch for release preparation, focus on that batch only. Test and fix its agreed improvements. Put new ideas and unrelated improvements in the backlog instead of expanding the release scope.

### 4. Verify before uploading

Install the release candidate in a fresh unpublished test copy and verify it before uploading to GitHub. Include the installation instructions in this verification.

The normal process must not be: upload, discover problems during testing, and upload again. Upload the verified candidate and its documentation together.

### 5. Preserve ownership

The merchant makes repository and theme edits unless explicitly delegated. Sidekick supplies small, sequential manual steps and may inspect saved work when asked. Preparing this agreement does not authorize repository edits.

## Proposed refinements: not yet adopted

These recommendations were discussed on 26 November 2026. Do not treat them as adopted until the merchant agrees.

### Definition of one improvement

An improvement is one complete, independently verifiable outcome that makes the component more useful, reliable, accessible, performant, or easier to install and maintain.

Count outcomes, not lines, files, or effort. A meaningful one-line fix can count. Multiple file changes delivering one outcome count as one improvement. Cosmetic or trivial edits should not be used to pad the count.

For each improvement, record:
- The outcome that changed.
- How it was checked and the result.

Example: making variant selection work correctly from a suggestion row is one improvement. The button, popup, and selected-variant handling are parts of that outcome, not automatically three improvements.

### Scope boundary

A component's scope includes the agreed customer experience, the foundations needed to deliver it, and the integration work required for those foundations to work together.

Ask: Is this work necessary to complete or verify the experience we agreed to build? A connection alone is not enough. Related opportunities that do not serve that experience go in the backlog.

### No quota-driven work

If agreed scope is complete with fewer than ten improvements, park the completed work and hold the normal release. Do not invent extra work or continue polishing just to reach ten.

### Test during production too

Check changes as they are built. The fresh-install verification is the final release gate, not the first time the improvements are tested. Freeze the candidate before final verification; if it changes, repeat the affected checks before uploading.

### Urgent-fix exception

A serious problem in an already released version may justify a focused fix below the normal ten-improvement threshold. This exception requires agreement; it is not an adopted exception yet.

## Suggested AGENTS.md reference

After this agreement is reviewed and placed in an agreed repository location, add a short reference in each relevant AGENTS.md rather than copying the full agreement into all three repositories:

> Follow the shared working agreement for component scope, meaningful improvement batches, release freezes, and test-before-upload requirements. Only its adopted rules are mandatory; proposed refinements require the merchant's agreement.

Include an explicit link to the chosen authoritative copy when adding this reference. If an older instruction conflicts with the adopted test-before-upload rules, update that instruction rather than leaving contradictory release procedures in place.
