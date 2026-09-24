# CLAUDE.md

@AGENTS.md

`AGENTS.md` (imported above) is the authoritative operating protocol: eligibility, links, duplicates, placement, formatting, triage decisions, validation, and protected areas. This file adds only Claude-specific orientation and repository facts. If the two conflict, follow `AGENTS.md` and flag the conflict.

## What This Repository Is

A curated Markdown list. `README.md` is the product; there is no application code, build, dependency install, linter, or test suite. Do not invent or install one.

| Path | Role |
| --- | --- |
| `README.md` | The list. Curation happens in `## Awesome Generative AI List` (around line 210 onward). |
| `Contributing.md` | Submission rules, including the repository threshold: more than 30 days old and at least 60 stars. |
| `Workflow.md` | Contributor fork-and-PR process. |
| `.github/workflows/claude.yml` | The only workflow: runs Claude when `@claude` is mentioned, with read-only `contents`, `pull-requests`, and `issues` permissions. No link checking, lint, or automatic review. |
| `.github/ISSUE_TEMPLATE/` | Generic bug, feature, and custom templates. There is no PR template. |
| `image/` | Banner and infographic assets. Protected. |
| `LINK_TO_*.md`, `Events.md`, `Projects.md`, `Resources.md` | Placeholder pages with `LINK_TO_…` stub links. Not part of curation; leave them alone unless asked. |

## README Structure

* Categories are `#####` headings under the main list, in roughly alphabetical order. Each ends with `**[⬆ back to top](#contents)**`; keep it after any added entry.
* Formats vary by section. Bullet sections use `* [Name](URL) - Description.`. Table sections have their own columns, such as Provider, Best For, Key Features, or Pricing. Copy the column order of the target table exactly.
* Many older entries break current style rules (for example, descriptions that start with "A"). Apply the rules to new or requested entries only; do not normalise neighbours.
* Known pre-existing issues, both in protected areas: `Recently Added` and `Connect with Us` hold stale or placeholder content. Mention these only when relevant, and fix them only when asked.

## Task Routing

* **PR or issue review**: read the diff or issue, then check it against `AGENTS.md`. Produce a recommendation, not edits, unless asked to edit.
* **Add or edit an entry**: read the target section and its neighbours first. Make the smallest edit that fits.
* **Broken-link sweep or multi-PR batch**: this is the one case where parallel subagents help. Split URLs or PRs across agents for link and duplicate checks, then consolidate the results yourself. For a single entry, work inline.
* **Instruction-file edits** (`CLAUDE.md`, `AGENTS.md`): keep them consistent with each other and with `Contributing.md`. Do not restate `AGENTS.md` here.

## Useful Commands

```text
grep -niE '<name>|<domain>|<owner>/<repo>' README.md   # duplicate search: name, URL, domain, aliases
git diff -U0 README.md                                  # confirm only intended lines changed
git diff --check                                        # whitespace errors
```

When you touch headings or anchors, list any `#` links that do not resolve. It should print `[]`:

```text
python3 -c "import re;t=open('README.md').read();s={re.sub(r'[^\w\- ]','',h.lower()).replace(' ','-') for h in re.findall(r'^#+\s+(.*?)\s*$',t,re.M)};print(sorted({l for l in re.findall(r'\]\(#([^)]+)\)',t)}-s))"
```

For table edits, check that the new row has the same number of `|` separators as the header row.

In cloud sessions, outbound requests go through a proxy. Blocked, rate-limited, or bot-protected responses are inconclusive; report them as unverified and do not treat them as broken.

## Review Output

For PR or issue reviews, report:

* **Decision**: accept, maintainer edit, request changes, close, or park.
* **Evidence**: 1–3 bullets, including the repository age and star count with the date checked where applicable, and any checks you could not complete.
* **Suggested entry** in the section's exact format, if the resource qualifies.
* **Maintainer comment**: a short, warm draft. Thank the contributor, state the decision and reason in one sentence, and point to the existing entry for duplicates.
* **Files changed**, if any.

A drafted comment is not a posted comment. Do not post, close, approve, or merge unless explicitly asked.
