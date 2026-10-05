# Learning record

This record documents the Codex agent's work on the NDHU practice repository. It is not a student's personal reflection or classroom observation.

- Tooling: Codex agent, GitHub CLI (`gh`), Git, PowerShell and Node.js.
- Route: Individual, agent-assisted local execution.
- Tasks: A folder organization, B activity picker (v1 and one revision), and D rejection.
- Scope: Only the task input data and corresponding output paths described in `submission-template.md` were used.

## Checks performed

1. A: found 12 source files and 12 manifest entries. Checked every output copy against its source with SHA-256; all matched. Identical files remained as separate copies, and both differing proposal versions remained.
2. B: exercised the required filters, no-match response, A09-only combination, five-item history cap, reset behavior, language switching and clear-history action in a local Node.js VM harness with a minimal DOM stub. All checked behaviors passed. Confirmed the HTML has no external script or stylesheet references.

## Revision

B v1 did not update the currently displayed activity name after switching languages. B v2 stores the selected activity and redraws it in the current language. The behavior harness confirmed the activity name changes language and history remains available.

## Rejection

Rejected the deliberately flawed plan to organize all Downloads, delete duplicates, infer the selected version from `final2`, guess missing values and publish automatically. The acceptable alternative stays within the selected practice folder, proposes changes before execution, preserves originals and differing versions, flags uncertainty, and does not publish.

## Not verified

No browser-based visual/mobile inspection or screenshot was captured. No personal student reflection or group code was supplied.
