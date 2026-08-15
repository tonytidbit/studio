<!--
SPDX-FileCopyrightText: 2026 copyright@bluem.studio
SPDX-License-Identifier: BSD-3-Clause
-->

# Studio work

[BLUEM STUDIO](https://bluem.studio/) files, their derivatives, and related
experiments.

## Agent instructions

These general instructions apply to every skill in this repository. Also follow
any additional agent instructions under the requested skill's section when
present.

Before installing or updating a skill, explain its purpose, behavior, source
material, dependencies, permissions, tools, network access, proposed scope,
and material risks, as applicable. Report its declared license, or report that
none was found. When updating, compare the installed skill with the requested
source and report material differences and local modifications. Install or
update the skill, then verify the result.

## After-Action Review

**Identifier:** `after-action-review`\
**Version:** `0.9.6` (2026-08-15)\
**Type:** Agent skill\
**Source:** [`skills/after-action-review/`](skills/after-action-review/)\
**Description:** A Codex CLI-first skill that audits a `/goal` against current
evidence before it is marked complete, then reviews what was requested, what
actually happened, why any discrepancy occurred, and what, if anything, should
be done differently next time. When installed as documented, the agent is
instructed to invoke it before completing each `/goal` and whenever the user
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

## Licensing

Licensing is declared per file using SPDX metadata. Full license texts are in
[`LICENSES/`](LICENSES/).
