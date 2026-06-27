# AGENTS.md

Operating protocol for AI coding agents working in this repository.

Claude Code should read `CLAUDE.md` first, then use this file as the shared repository contract. Other agents should start here. Follow repository-local guidance over generic awesome-list assumptions.

## Repository North Star

This is a public, maintained awesome list for generative AI. The `README.md` is the product: a durable, high-signal, navigable map of the field for readers, contributors, and AI agents.

The list is curated, not accumulated. Each entry should help a reader understand the generative AI landscape, find a credible resource, or compare related tools. Selectivity, durability, clear placement, and neutral description quality matter more than volume.

## Agent Role

Agents may help with:

* README maintenance when explicitly asked
* New entry review
* Pull request review
* Issue triage
* Broken-link checks
* Duplicate detection
* Section placement
* Description tightening
* Maintainer comment drafts
* Small, safe cleanup edits when explicitly requested

Agents must not:

* Add speculative or low-signal entries
* Inflate claims or preserve promotional wording
* Reorganise the list without explicit instruction
* Run broad formatting sweeps
* Edit unrelated files
* Rewrite the maintainer’s style unnecessarily
* Turn one contribution into a broad structural change
* Touch protected areas unless explicitly instructed

## Read Order

Before reviewing or editing, read in this order:

1. `README.md` — scope, taxonomy, formatting, protected areas, and existing examples
2. `Contributing.md` — submission requirements and entry format
3. `Workflow.md` — PR process, if relevant
4. `.github/ISSUE_TEMPLATE/` — contributor expectations
5. `.github/PULL_REQUEST_TEMPLATE.md`, if present
6. `CLAUDE.md`, if the agent is Claude Code or needs Claude-specific review format
7. Recent issues and merged PRs, where available, for maintainer precedent

Do not assume the generic awesome-list pattern overrides this repository’s existing structure.

## Repository Facts

* The `README.md` contains introductory sections, Contents, Recently Added, infographics, and the main “Awesome Generative AI List”.
* Main list sections use a mixture of bullets and tables. Match the local section style exactly.
* Some sections include explanatory text before entries. Preserve it.
* `Contributing.md` sets hard gates for many repository-style submissions: the project should be more than 30 days old and have at least 60 stars.
* `Contributing.md` asks for one PR per suggestion.
* New entries should be added to the bottom of the relevant category unless local ordering clearly indicates otherwise.
* New categories or category improvements should be handled separately.
* For package-style submissions, prefer the GitHub repository over a package registry or marketing page.
* Descriptions should be short, simple, descriptive, and non-promotional.

## Scope Rules

Belongs:

* Official repositories
* Official documentation
* Papers and technical reports
* Datasets and benchmarks
* Evaluation tools
* Agent frameworks and orchestration tools
* RAG and retrieval resources
* AI-native development tools
* Generative media tools
* Durable tutorials, courses, books, and technical explainers
* Safety, alignment, observability, tracing, testing, and security resources relevant to generative AI
* High-signal platforms, libraries, frameworks, standards, and reference resources

Does not belong:

* Thin wrapper pages with little original technical value
* Pure marketing pages
* Broken or inaccessible links
* Duplicate or near-duplicate resources
* Speculative entries
* Low-signal directories or link farms
* Unsupported ranking, performance, adoption, or novelty claims
* Pricing claims unless the surrounding section already tracks pricing
* Time-sensitive claims such as “latest”, “best”, “leading”, “fastest”, or “most advanced”
* Content outside generative AI or adjacent technical areas already represented in the README

## Quality Bar

An entry qualifies when all are true:

* It is clearly relevant to generative AI or an adjacent technical area already represented in the list.
* The source is credible and useful to a technical reader.
* The link is canonical, durable, and reachable.
* The resource adds something distinct from existing entries.
* The entry fits an existing section without forcing a taxonomy change.
* The description is neutral, concise, specific, and non-promotional.
* The formatting matches the surrounding section.
* No duplicate or stronger existing equivalent is already present.

## README Formatting Rules

Infer format from the surrounding section before editing.

* Preserve the existing heading structure.
* Preserve all back-to-top links and anchors.
* Preserve badges, banners, infographics, Contents, Recently Added, contributor sections, and other protected areas.
* Match the section’s existing format: bullet list, table, heading, or grouped subsection.
* Use HTTPS links where available.
* Use canonical names.
* Keep descriptions short.
* Start descriptions with a capital letter.
* End descriptions with a full stop.
* Do not use title case for descriptions.
* Do not start descriptions with “A” or “An”.
* Do not perform broad formatting changes unless explicitly asked.

## Link Quality Rules

Verify that:

* The link resolves.
* The link points to the canonical source.
* Repository links point to the main project, not an arbitrary fork.
* Paper links prefer official publisher pages, arXiv, DOI, or project pages.
* Documentation links prefer official docs.
* Dataset links prefer official dataset pages or maintained repositories.
* URLs do not include avoidable tracking parameters.
* Login-gated resources are avoided unless the list already accepts that kind of resource.
* Shortened links are avoided.

## Description Style

Descriptions should be:

* Neutral
* Factual
* Specific
* Short
* Present tense where possible
* Free of hype
* Free of unsupported claims
* Useful to a reader scanning the list quickly

Prefer:

* “Framework for evaluating LLM agents across task environments.”
* “Dataset for benchmarking retrieval-augmented generation systems.”
* “Open-source tool for tracing agent execution and debugging tool calls.”
* “Platform for building and deploying multi-agent workflows.”

Avoid:

* “Powerful”
* “Revolutionary”
* “Cutting-edge”
* “Best”
* “Latest”
* “Industry-leading”
* “Game-changing”
* “Fastest”
* Unsupported claims about performance, adoption, or maturity

## Section Placement Rules

1. Identify the closest existing section.
2. Compare the candidate with neighbouring entries.
3. Prefer the narrowest accurate section.
4. If two sections fit, choose the one where readers would most naturally look first.
5. Avoid creating a new section for a single item.
6. Do not move many existing entries unless explicitly asked.
7. If placement is uncertain, state the trade-off and recommend one option.
8. New category proposals should usually be separate from single-entry PRs.

## Duplicate Checking Rules

Before adding or approving, check for:

* Same URL
* Same project under a different URL
* Same paper title
* Same organisation and product name
* Renamed repositories
* Existing entry in a nearby section
* Existing issue or PR suggesting the same resource
* A stronger canonical source already listed

If a duplicate exists, recommend closing, editing, or redirecting rather than adding another entry.

## Decision Matrix

| Decision           | Use when                                                                                                  |
| ------------------ | --------------------------------------------------------------------------------------------------------- |
| Accept as-is       | In scope, canonical link, correct placement, matching format, neutral description, no duplicate.          |
| Edit as maintainer | Strong resource needing small fixes: wording, punctuation, canonical URL, placement, or local formatting. |
| Request changes    | Resource may fit but evidence, link quality, relevance, or placement is materially unclear.               |
| Close              | Out of scope, duplicate, promotional, broken with no replacement, or no durable technical substance.      |
| Park               | Promising but immature, not yet supported by the taxonomy, or requires maintainer judgement.              |

## Issue-to-Entry Workflow

For suggestion issues:

1. Check scope.
2. Check source quality.
3. Check link quality.
4. Check duplicates.
5. Identify the best section.
6. Draft a neutral entry only if the resource qualifies.
7. Recommend accept, maintainer edit, request changes, close, or park.
8. Keep the maintainer comment concise.

For broken-link issues:

1. Verify the reported link.
2. Search for a canonical replacement.
3. Prefer official replacements over mirrors.
4. Preserve the entry if a durable replacement exists.
5. Recommend removal only when no credible replacement exists.
6. State the action clearly.

## Pull Request Review Workflow

1. Read the PR title, description, and diff.
2. Confirm it changes only relevant files.
3. Check each added or changed link.
4. Check scope and source quality.
5. Check duplicates.
6. Check section placement.
7. Check local formatting.
8. Neutralise description language where needed.
9. Decide: accept, maintainer edit, request changes, close, or park.
10. Draft a concise maintainer comment.

Minimise contributor friction. If the resource is clearly suitable and the issue is minor, recommend a maintainer edit rather than asking the contributor to revise.

## Stop and Ask

Stop and ask the maintainer before:

* Creating a new top-level section
* Reordering large parts of the README
* Changing the Contents structure
* Editing Recently Added
* Editing infographics, banners, badges, or visual assets
* Changing contribution rules
* Removing multiple entries
* Making judgement-heavy scope changes
* Editing files unrelated to the stated task

## Protected Areas

Do not edit unless explicitly instructed:

* Badges
* Banner images
* Gallery images
* Infographics
* Contents
* Recently Added
* Announcement or roadmap blocks
* Contributor lists
* Generated indexes
* Licence text
* Repository metadata unrelated to the task
* Private notes
* Draft files
* Scratch files
* Local-only files

## Maintainer Comment Style

Comments should be warm, concise, respectful, and decision-oriented.

Prefer:

* “Thank you for the suggestion. This is relevant, the link is canonical, and I would place it under X with a shorter neutral description.”
* “Thank you — useful resource. I would accept this with a small maintainer edit to remove the ranking claim.”
* “Thank you for raising this. I would close it as a duplicate because the resource already appears under X.”
* “Thank you — I would park this for now until the list has a clearer section for this category.”

Avoid:

* Long explanations
* Harsh rejection wording
* Defensive language
* Asking contributors for trivial edits the maintainer can safely make

## Final Response Pattern

When finishing a task, summarise:

* What was reviewed
* Decision or recommended decision
* What changed, if anything
* Any risks or uncertainties
* Suggested maintainer comment, if relevant
* Follow-up needed, if any

Do not modify `README.md` or other files unless explicitly asked.
