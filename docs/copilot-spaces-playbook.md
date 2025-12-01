# Copilot Spaces Playbook

## Purpose
This playbook explains how to use Copilot Spaces to scale institutional knowledge for the OctoAcme project. It includes a recommended article template, ownership and review practices, example prompts, and suggestions for repository structure so Spaces can surface high-quality content.

## Why this matters
- Centralizes knowledge so new hires and cross-functional collaborators onboard faster.
- Makes institutional context queryable in Copilot Spaces and other knowledge tools.
- Ensures accuracy via lightweight ownership and review cadence.

## Recommended article metadata (frontmatter)
Add a short YAML frontmatter to each knowledge article so Spaces and humans can quickly scan and filter content.

Example:

```yaml
title: "How we run release checklists"
summary: "Checklist and ownership for every OctoAcme release"
owners:
  - team: "platform"
  - contact: "@release-lead"
tags:
  - release
  - checklist
  - ops
created: 2025-12-01
review_date: 2026-06-01
status: stable # draft | stable | deprecated
```

## Article structure (template)
- **Problem**: One-sentence description of the problem this doc solves.
- **Context / When to use**: Scenarios where this guidance applies.
- **Steps / Playbook**: Numbered, actionable steps with expected outcomes.
- **Examples**: Short examples or snippets.
- **Related**: Links to other docs, PRs, or issues.
- **Change history**: Who updated and why.

Copyable template (start your article with the YAML then the sections above):

````markdown
---
title: "<Short title>"
summary: "<1-line what this doc is about>"
owners:
  - team: ""
  - contact: ""
tags: ["", ""]
created: YYYY-MM-DD
review_date: YYYY-MM-DD
status: draft
---

# <Short title>

## Problem

## Context / When to use

## Steps / Playbook

## Examples

## Related

## Change history
````

## How to publish and maintain articles
- Create a branch and open a PR against `main` with your new or updated article.
- Assign the article owner as a reviewer and add the `docs` label.
- After owner review and one additional reviewer, merge to `main`.
- Set `review_date` for periodic validation (e.g., 6 months).

## Getting the most from Copilot Spaces
- Put the canonical content in `docs/` (or a dedicated `knowledge/` folder).
- Add short, focused articles rather than extremely long pages—atomic articles are easier for Spaces to surface.
- Consider adding a `.copilot/` folder with project-specific prompts, templates, and context snippets. Copilot Spaces will use repo context to improve suggestions.
- Use consistent tags and frontmatter so Spaces can filter by `team`, `topic`, and `status`.

## Example prompts for teammates
- "Show me the release checklist for OctoAcme"
- "How do I create a Project One-pager in this repo?"
- "What are the acceptance criteria for our release process?"

## Ownership and governance
- Each article must have at least one owner listed in the `owners` metadata.
- Owners are responsible for verifying and updating content by `review_date`.
- Maintain a `docs/OWNERS.md` if you want centralized ownership mapping.

## Metrics and signals of quality
- Number of views / queries (if available in Spaces analytics).
- Number of edits and review cycles.
- Feedback from reviewers and consumers (short thumbs-up or quick issues).

## Suggested next steps for this repo
- Add a few seed articles following the template.
- Optionally add `.copilot/` prompts focused on onboarding and common workflows.
- Configure owner review cadence (e.g., quarterly or semi-annual reviews).

--
This playbook is a lightweight starting point. Tailor the fields and cadence to your teams' needs.
