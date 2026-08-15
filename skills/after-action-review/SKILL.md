---
# SPDX-FileCopyrightText: 2026 copyright@bluem.studio
# SPDX-License-Identifier: BSD-3-Clause
name: after-action-review
description: Audit a /goal against current authoritative evidence before it is marked complete, then conduct a concise after-action review; also use when the user requests an AAR, a review of completed work, or lessons from a period of work.
license: BSD-3-Clause
metadata:
  publisher: "BLUEM STUDIO <https://bluem.studio/>"
  version: "0.9.6"
---

# Studio After-Action Review

## Goal Completion Audit

When invoked because a `/goal` appears ready to conclude, first verify
completion.

Extract every explicit requirement and map it to current authoritative evidence.
Classify each requirement as:

- proven
- contradicted
- incomplete
- unverified

Do not treat tests, effort, plausible output, or partial progress as proof.

If any requirement is contradicted, incomplete, or unverified, do not conclude
the goal. Continue working when possible; otherwise, report the accurate
non-complete state.

Once completion is proven, conclude the goal and perform the after-action review
below.

Manually requested AARs should remain retrospective and should not resume work
unless requested.

## After-Action Review

Review the work just completed. Scope the review to:

1. The concluded `/goal`, when applicable.
2. The period or work identified by the user.
3. Otherwise, the narrowest reasonable scope supported by the current context,
   stated explicitly.

Answer these four questions:

1. What was supposed to happen, or what was requested?
2. What actually happened?
3. Why was there a discrepancy?
4. What should be done differently next time?

Base each answer on observable results and known context. Distinguish the user's
contributions from the agent's. If there was no material discrepancy, say so
instead of inventing one. Keep the review proportional to the work.

Do not silently expand the scope or treat unfinished work as complete.
Assess the requested outcome rather than rewarding effort, generic capability,
or unrelated improvements.

Finish with a `TL;DR` section summarizing the overall assessment and the most
important change for next time.
