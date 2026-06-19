[English](README.md) · [العربية](i18n/README.ar.md) · [Español](i18n/README.es.md) · [Français](i18n/README.fr.md) · [日本語](i18n/README.ja.md) · [한국어](i18n/README.ko.md) · [中文 (简体)](i18n/README.zh-Hans.md) · [中文（繁體）](i18n/README.zh-Hant.md) · [Deutsch](i18n/README.de.md)

[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://lazying.art)

# Paper Critique Skill

**Strict reviewer-style critique for academic manuscripts, grant proposals, pre-proposals, PDFs, DOCX files, and LaTeX submissions.**

[![Website](https://img.shields.io/badge/Website-lazying.art-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://lazying.art)
[![GitHub](https://img.shields.io/badge/GitHub-lachlanchen-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/lachlanchen)
[![Skill](https://img.shields.io/badge/Codex-Skill-2563eb?style=for-the-badge&logo=openai&logoColor=white)](SKILL.md)
[![Companion](https://img.shields.io/badge/Companion-Paper%20Revision%20Skill-16a34a?style=for-the-badge&logo=readthedocs&logoColor=white)](https://github.com/lachlanchen/paper-revision-skill)

Paper Critique Skill helps Codex act like a demanding academic reviewer:

> **Read the submission as a reviewer. Find the weak points. Write actionable comments.**

It is designed for deep review before revision: manuscript flaws, grant-readiness risks, methodological gaps, claim/evidence mismatches, formal compliance issues, funder fit, reviewer-confidence risks, and LaTeX/PDF review-comment documents.

## Companion Skill

Use the two paper skills together:

| Need | Use |
| --- | --- |
| Review, critique, score, challenge, or generate reviewer-style comments | **Paper Critique Skill** |
| Revise manuscript text, answer reviewer comments, produce response letters, build redlines, or prepare submission packages | [**Paper Revision Skill**](https://github.com/lachlanchen/paper-revision-skill) |

Typical flow:

```text
Draft manuscript or proposal
        |
        v
Paper Critique Skill
  deep review comments
        |
        v
Paper Revision Skill
  response letter + revised manuscript + redline
```

## Why This Exists

Good critique is different from good revision. A reviewer should not immediately rewrite the manuscript. First, they should identify what could block acceptance, lower the score, damage credibility, or confuse a panel.

This skill separates review from revision:

| Phase | Purpose | Artifact |
| --- | --- | --- |
| Source freeze | Identify PDF, DOCX, TeX, forms, instructions, prior comments | review source map |
| Extraction | Recover visible and hidden reviewable text | extracted text or notes |
| Compliance audit | Check placeholders, word limits, empty fields, comments, tracked changes | formal-risk list |
| Deep critique | Challenge claim, novelty, evidence, feasibility, fit, and writing | reviewer-style comments |
| Output | Write structured comments in Markdown or LaTeX/PDF | review-comment document |

## Quick Start

```text
Use $paper-critique-skill to review this manuscript like a strict reviewer.
Find formal, scientific, feasibility, and presentation flaws.
Write detailed comments with severity, location, why it matters, and required fixes.
If useful, compile the comments to PDF.
```

For a grant pre-proposal:

```text
Use $paper-critique-skill to critique this Veni/ERC/NIH proposal.
Check eligibility-visible fields, funder fit, applicant independence, output evidence, feasibility, and reviewer confidence.
Do not edit the manuscript yet.
```

## What Is Included

| Path | Use |
| --- | --- |
| [`SKILL.md`](SKILL.md) | Active Codex skill instructions |
| [`agents/openai.yaml`](agents/openai.yaml) | UI metadata for Codex skill listings |
| [`references/review-comment-rubric.md`](references/review-comment-rubric.md) | Deep review lenses and severity calibration |
| [`assets/deep-review-comments-template.tex`](assets/deep-review-comments-template.tex) | LaTeX template for detailed review-comment PDFs |
| [`i18n/`](i18n/) | Multilingual README summaries |

## Review Lenses

| Lens | What the reviewer challenges |
| --- | --- |
| Formal compliance | visible instructions, empty fields, placeholders, word limits, required sections |
| Central claim | hypothesis, novelty, fit, audience, contribution |
| Evidence chain | support for claims, citations, preliminary data, controls, overclaiming |
| Methods and feasibility | aims, go/no-go criteria, model choice, risk controls, endpoints |
| Reviewer confidence | independence, team roles, host infrastructure, execution realism |
| Writing and packaging | structure, clarity, figure/table logic, reviewer-facing polish |

## Comment Format

Strong comments are specific and actionable:

```text
ID: S2
Severity: Major
Location: Research idea, Aim 2
Concern: The receptor strategy lists multiple architectures without naming a first-line construct.
Why it matters: Reviewers cannot judge feasibility or success criteria.
Required fix: Name the primary construct, fallback, and minimal go/no-go readout.
```

## Topics And URLs

Suggested GitHub topics:

`codex-skill`, `academic-writing`, `peer-review`, `manuscript-review`, `grant-review`, `latex`, `pdf`, `docx`, `reviewer-comments`, `research-assessment`

Project URLs:

- Skill repository: <https://github.com/lachlanchen/paper-critique-skill>
- Companion revision workflow: <https://github.com/lachlanchen/paper-revision-skill>
- Website: <https://lazying.art>
- Chat/donation page: <https://chat.lazying.art/donate>

## Install

Clone into your Codex skills folder:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
git clone https://github.com/lachlanchen/paper-critique-skill.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/paper-critique-skill"
```

Then ask Codex:

```text
Use $paper-critique-skill to write a deep reviewer-style critique of this paper.
```

## Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://img.shields.io/badge/Donate-LazyingArt-0EA5E9?style=for-the-badge&logo=kofi&logoColor=white)](https://chat.lazying.art/donate) | [![PayPal](https://img.shields.io/badge/PayPal-RongzhouChen-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/RongzhouChen) | [![Stripe](https://img.shields.io/badge/Stripe-Donate-635BFF?style=for-the-badge&logo=stripe&logoColor=white)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |

## Contact

[![Website](https://img.shields.io/badge/Website-lazying.art-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://lazying.art)
[![Email](https://img.shields.io/badge/Email-lach@lazying.art-0ea5e9?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lach@lazying.art)
[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-lachlanchen-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/lachlanchen)

Review harder. Revise cleaner.
