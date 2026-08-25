<!--
SPDX-FileCopyrightText: 2026 copyright@bluem.studio
SPDX-License-Identifier: BSD-3-Clause
-->

# Studio work

[BLUEM STUDIO](https://bluem.studio/) files, their derivatives, and related
experiments.

## Agent instructions

These instructions apply to every installable item in this repository. Also
follow any item-specific instructions under the requested item's section.

Inspect the existing state and map each requested item to an exact target and
scope. Install or update only the resolved targets. Verify their contents and
effective scope and, as applicable, discovery, activation, and persistence.

For each item, report its type, source, license status, expected behavior, and
material impact, including consequential dependencies, permissions, tools, or
network access. Also report material differences and local modifications
compared with any existing installation.

Do not proceed without user confirmation if a target or scope is ambiguous or
the proposed installation could create a conflict. For an aggregate request,
present the target and scope of every included item before making changes.

## After-Action Review

**Identifier:** `after-action-review`\
**Version:** `0.9.7` (2026-08-25)\
**Type:** Agent skill\
**Source:** [`skills/after-action-review/`](skills/after-action-review/)\
**Description:** A Codex CLI-first skill that audits a `/goal` against current
evidence before it is marked complete, then reviews what was requested, what
actually happened, why any discrepancy occurred, and what, if anything, should
be done differently next time. When invoked for goal completion or at the
user's request, its four-part review appears in the final response, while the
framework may also be used internally. When installed as documented, the agent
is instructed to invoke it before completing each `/goal` and whenever the user
requests an after-action review, optionally scoped by the user.

To install or update, tell your AI agent:

> Install or update `after-action-review` from `https://github.com/tonytidbit/studio`.

### Additional agent instructions

Also configure and verify the applicable agent instructions to invoke the skill
before marking a `/goal` complete and whenever the user requests an after-action
review.

## Startup Review

**Identifier:** `startup-review`\
**Version:** `0.11.0` (2026-08-15)\
**Type:** Agent skill\
**Source:** [`skills/startup-review/`](skills/startup-review/)\
**Description:** Reviews a startup's foundations using Guy Kawasaki's ten-slide
framework and the Business Model Canvas through stakeholder questions and a
dated working model. Full reviews account for every framework item, classify the
strength of each answer, identify supporting evidence, and reconcile the results
into focused questions and prioritized decisions.

To install or update, tell your AI agent:

> Install or update `startup-review` from `https://github.com/tonytidbit/studio`.

## TL;DR

**Identifier:** `tldr`\
**Version:** `0.1.0` (2026-08-25)\
**Type:** Agent instruction\
**Source:** This README section\
**Description:** Adds a concise concluding summary to long agent responses so
the reader can understand the main conclusion, any material qualification, and
the next action without carefully processing the complete response.

To install or update, tell your AI agent:

> Install or update the `tldr` instruction from
> `https://github.com/tonytidbit/studio` as a user-wide instruction for this AI,
> unless another scope is given. Add or update only the `## TL;DR` instruction,
> preserve unrelated configuration, and verify that it persists.

### Instruction

```markdown
## TL;DR

For final responses of roughly 600 words or more, end with a `TL;DR` of no more
than 50 words that lets the reader understand the answer without reading the
full response. State the main conclusion, any qualification that materially
changes it, and the next action when applicable. Do not introduce new
information. Omit the section when the user requests another format.
```

### Installation and removal

Use the persistent instruction mechanism appropriate to the AI and requested
scope. To remove the instruction, remove only the installed `## TL;DR`
instruction and preserve unrelated configuration.

## Licensing

Licensing is declared per file using SPDX metadata. Full license texts are in
[`LICENSES/`](LICENSES/).
