---
name: paper-critique-skill
description: Rigorous academic manuscript and grant-proposal critique workflow for producing reviewer-style comments, deep flaw audits, funder-readiness assessments, and LaTeX/PDF review-comment documents. Use when Codex is asked to review, critique, referee, challenge, score, or write detailed reviewer comments on a paper, proposal, pre-proposal, response draft, DOCX, PDF, or LaTeX manuscript without necessarily editing the manuscript itself.
---

# Paper Critique Skill

## Companion Skill Boundary

Use this skill to critique and write review comments. Use `paper-revision-skill` instead when the user asks to revise manuscript text, answer reviewer comments, update response letters, generate redlines, or prepare a submission package.

When both are requested, critique first with this skill, then switch to the revision workflow before editing manuscript sources.

The intended pair is:

- `paper-critique-skill`: review the paper, proposal, PDF, DOCX, or TeX source and produce rigorous critique comments.
- `paper-revision-skill`: respond to those comments, revise the manuscript, build PDFs, generate redlines, and prepare submission-ready response packages.

## Workflow

1. Freeze the source set: identify DOCX, PDF, TeX, bibliography, figures, forms, instructions, word limits, and any prior review comments.
2. Extract the reviewable text from the most authoritative source. Prefer compiled PDF text for what a reviewer sees; use TeX/DOCX to recover structure, comments, and hidden metadata.
3. Check formal compliance before science: visible instructions, empty fields, word limits, placeholders, required sections, references, captions, and administrative declarations.
4. Read like a skeptical expert reviewer. Challenge the central claim, novelty, evidence chain, feasibility, risk controls, methods, outcome measures, independence, writing structure, and fit to the funder or journal.
5. Separate problems by severity:
   - Critical: likely to block submission, eligibility, credibility, feasibility, or reviewer confidence.
   - Major: materially weakens score, persuasiveness, interpretation, novelty, or execution.
   - Minor: wording, presentation, local clarity, or polish.
6. Write actionable comments. Each comment should state the problem, why it matters, what evidence or revision would fix it, and where the issue appears.
7. Do not invent facts, preliminary data, citations, eligibility details, or reviewer requirements. Mark unknowns explicitly.
8. If outputting LaTeX comments, compile and inspect the PDF when a build toolchain is available.

## Comment Style

Use a direct, reviewer-like tone: firm, specific, and fair. Avoid vague praise. Do not soften severe issues when the source would genuinely concern a reviewer.

Prefer this structure for detailed comment documents:

1. Context and source basis.
2. Overall verdict from a strict reviewer.
3. Top-priority problems.
4. Detailed reviewer-style comments grouped by severity and theme.
5. Submission-risk checklist or action table.
6. Closing recommendation.

For individual comments, use stable IDs such as `F1`, `F2`, `S1`, `M1`, where:

- `F` = formal/compliance issue.
- `S` = scientific or scholarly issue.
- `M` = methods, feasibility, management, or measurement issue.
- `P` = presentation, writing, or packaging issue.

Each comment should contain:

- Severity.
- Location or anchor.
- Reviewer concern.
- Why it matters.
- Required fix.

## Review Lenses

Read `references/review-comment-rubric.md` when writing a deep critique or when the source is a grant, pre-proposal, or manuscript with many moving parts.

Use `assets/deep-review-comments-template.tex` as the starting format when the user asks for review comments in LaTeX/PDF form.

## Verification

For TeX/PDF outputs:

- Compile the comment document if possible.
- Use `pdftotext -layout` to confirm the verdict, top-priority problems, comment IDs, and disclosure/footer appear in the PDF.
- Record build warnings that may affect readability.

For DOCX/PDF sources:

- Report whether tracked changes, Word comments, or PDF text annotations were found.
- Do not claim comments or tracked changes exist unless detected in the file structure.
