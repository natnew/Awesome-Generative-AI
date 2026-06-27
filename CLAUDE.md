# CLAUDE.md

This file guides Claude Code when working in this repository.

This repository is a public, maintained awesome list for generative AI, not an application codebase. There is no build, lint, or test workflow to run for normal review tasks. The `README.md` is the product.

Claude Code should read this file first, then use `AGENTS.md` as the shared repository operating protocol.

## North Star

* Preserve `README.md` as the canonical public artefact.
* Keep the list selective, durable, technically useful, neutral, and easy to scan.
* Help the maintainer make fast, consistent, low-friction decisions.
* Prefer small, precise edits over broad rewrites.
* Do not broaden the list beyond generative AI and clearly adjacent technical areas already represented in the README.

## Claude’s Role

Claude may assist with:

* PR review
* Issue triage
* README entry review
* Broken-link investigation
* Duplicate detection
* Section placement
* Neutral description rewrites
* Maintainer comment drafts
* Small safe maintainer edits when explicitly asked
* Improvements to agent instruction files when asked

Claude must not:

* Add entries without checking scope, link quality, duplicates, and placement
* Invent facts about a resource
* Preserve promotional claims
* Add ranking, pricing, novelty, adoption, or performance claims without strong evidence
* Rewrite the taxonomy without explicit instruction
* Edit unrelated files
* Touch protected areas unless instructed
* Ask contributors to make trivial fixes the maintainer can safely make

## Repository Facts

* `AGENTS.md` contains the full tool-agnostic operating protocol.
* `Contributing.md` contains contributor-facing rules.
* `Workflow.md` contains PR process detail.
* `.github/ISSUE_TEMPLATE/` contains public issue guidance.
* The `README.md` contains introductory content, Contents, Recently Added, infographics, and the main “Awesome Generative AI List”.
* The main list uses both bullet entries and tables. Match the surrounding section exactly.
* New entries usually go to the bottom of the relevant category unless local ordering clearly indicates otherwise.
* New categories should normally be handled separately.
* Protected areas include badges, Contents, Recently Added, banners, images, infographics, contributor blocks, generated sections, and licence text.

## Always-Loaded Context

Keep this file short. It is an orientation layer, not a manual.

Use this routing:

* Need general agent rules → read `AGENTS.md`
* Need contribution rules → read `Contributing.md`
* Need PR process → read `Workflow.md`
* Need style examples → inspect the target section in `README.md`
* Need contributor expectations → inspect `.github/ISSUE_TEMPLATE/`
* Need maintainer precedent → inspect recent issues and merged PRs where available

Do not duplicate long sections from those files here.

## First-Pass Workflow

For any PR, issue, or README task:

1. Read the user request.
2. Read the relevant issue, PR, diff, or target README section.
3. Check the repository scope.
4. Check `Contributing.md` if the task concerns a submission.
5. Check neighbouring entries for style and placement.
6. Search for duplicates.
7. Verify the link where tools allow.
8. Inspect the resource enough to understand what it is.
9. Choose the smallest useful action.
10. Produce a concise decision, edit, or maintainer comment.

## Entry Checklist

Before recommending acceptance or adding an entry, confirm:

* In scope
* Technically useful
* Credible source
* Canonical URL
* Durable link
* No duplicate
* Correct section
* Local format matched
* Neutral description
* No hype
* No unsupported claims
* No avoidable tracking parameters
* No unnecessary new section

## Source Preference

Prefer:

* Official repositories
* Official documentation
* Papers
* Technical reports
* Benchmarks
* Datasets
* Durable project pages
* Maintained tools and libraries
* High-quality reference material

Treat cautiously:

* Launch posts
* Vendor pages
* Thin wrappers
* Newsletter posts
* Social posts
* Unmaintained repositories
* Link farms
* Pages dominated by sales language
* Time-sensitive comparisons

## Description Rules

Default pattern:

`* [Name](URL) - Clear factual description.`

For tables, preserve the existing column structure.

Descriptions should:

* Start with a capital letter
* End with a full stop
* Be short and specific
* Avoid title case
* Avoid starting with “A” or “An”
* Avoid marketing taglines
* Explain what the resource is, not why it is exciting

Remove or neutralise:

* “best”
* “latest”
* “most advanced”
* “powerful”
* “revolutionary”
* “cutting-edge”
* “game-changing”
* “industry-leading”
* “fastest”
* Unsupported performance, adoption, maturity, or pricing claims

## Section Placement

| Situation                             | Action                                                |
| ------------------------------------- | ----------------------------------------------------- |
| Exact fit in an existing section      | Place there.                                          |
| Fits two sections                     | Choose the more specific or more discoverable one.    |
| Similar to neighbouring entries       | Place near those entries if local ordering allows.    |
| New theme with one entry              | Park, or place in the nearest broader section.        |
| New theme with several strong entries | Suggest a new section; do not create it unless asked. |
| Unclear placement                     | Explain the options briefly and recommend one.        |

## PR Triage

| Decision        | Use when                                                                                  |
| --------------- | ----------------------------------------------------------------------------------------- |
| Accept as-is    | Scope, link, placement, format, and description are all sound.                            |
| Maintainer edit | Strong resource needing only minor wording, link, placement, or formatting fixes.         |
| Request changes | Relevance, evidence, link quality, or placement is materially unclear.                    |
| Close           | Out of scope, duplicate, promotional, broken with no replacement, or low technical value. |
| Park            | Promising but immature, needs a taxonomy decision, or needs maintainer judgement.         |

## Issue Triage

Suggestion issues:

* Strong, in scope, canonical → draft entry and recommend acceptance.
* Strong but wording or placement needs work → recommend maintainer edit.
* Missing evidence → ask for minimal clarification.
* Duplicate → close with a pointer to the existing entry.
* Out of scope → close politely.
* Premature or taxonomy-dependent → park.

Broken-link issues:

* Verify the link.
* Find a canonical replacement first.
* Prefer official sources over mirrors.
* Remove only when no durable replacement exists.
* Leave a concise note explaining the action.

## Small Safe Fix Rule

Protect contributor goodwill.

When a resource is suitable and the issue is minor, make or recommend a maintainer edit rather than asking the contributor to revise.

Small safe fixes include:

* Tightening a description
* Removing hype
* Fixing punctuation
* Correcting placement
* Replacing a non-canonical URL
* Matching bullet or table format
* Removing tracking parameters

## Stop and Ask

Stop before:

* Creating a new top-level section
* Reordering large parts of the README
* Editing Contents
* Editing Recently Added
* Editing visual assets
* Changing contribution rules
* Removing several entries
* Making broad scope decisions
* Editing unrelated files

## Protected Areas

Do not edit unless explicitly instructed:

* Badges
* Contents
* Recently Added
* Banner images
* Gallery images
* Infographics
* Announcement or roadmap blocks
* Contributor sections
* Generated indexes
* Licence text
* Repository metadata unrelated to the task
* Private, draft, scratch, or local-only files

## Maintainer Comment Templates

Accept:

“Thank you — this looks relevant, the link is canonical, and the placement works. I would accept this.”

Maintainer edit:

“Thank you — this is a useful resource. I would accept it with a small maintainer edit to tighten the description and keep the wording neutral.”

Request changes:

“Thank you for the suggestion. I think this could fit, but I would ask for a little more context on why this is the canonical source and where it belongs.”

Duplicate:

“Thank you — I would close this as a duplicate because the resource already appears under [section].”

Out of scope:

“Thank you for sharing this. I would close it because it sits outside the current scope of the list.”

Park:

“Thank you — this may be worth revisiting, but I would park it for now until the list has a clearer section for this category.”

## Output Format

For PR or issue review, respond with:

* **Decision**: accept, maintainer edit, request changes, close, or park
* **Reason**: 1–3 bullets
* **Suggested README entry**, if useful
* **Suggested maintainer comment**
* **Files changed**, if any
* **Remaining uncertainty**, if any

## Editing Rule

Do not modify `README.md`, `Contributing.md`, `.github` templates, or other files unless explicitly asked.
