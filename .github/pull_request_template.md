##What changed
Added a PR template at .github/pull_request_template.md (What/Why/How to test + checklist).
Added a personal pre-PR self-review checklist at docs/pr-checklist.md.
Updated README.md with a How to run section for local setup on Windows/PowerShell.

##Why
To standardize PR descriptions and make reviews faster and clearer (context + verification steps).
To reduce common PR problems: vague titles, missing rationale, scope creep, and non-reproducible changes.

##How to test
Open GitHub → create a new PR → confirm the description auto-fills from the PR template.
Verify files exist and contain content:
Get-Content .github\pull_request_template.md
Get-Content docs\pr-checklist.md
Confirm README contains the section:
Select-String -Path README.md -Pattern "How to run"
Expected: template content appears, checklist has 5+ - [ ] items, and README includes “How to run”.

##Notes / Risks
Documentation/process-only change; no runtime behavior impact.
No migrations, feature flags, or backwards-compatibility concerns.

##Checklist
 Title is specific and in imperative mood (e.g., "docs: add …", "fix: correct …")
 PR is one logical change (no unrelated refactors/formatting)
 Instructions are reproducible (a reviewer can verify in <5 minutes)
 Tests added/updated OR I explained why not (N/A — docs/template change)
 README/docs updated if behavior changed
 No debug artifacts left (print/breakpoint/commented code)
