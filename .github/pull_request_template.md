##What changed
Added PR template: .github/pull_request_template.md
Added self-review checklist: docs/pr-checklist.md
Added How to run section to README.md

##Why
To standardize PR info and make reviews easier (clear What/Why/How to test).

##How to test
Open a new PR and confirm the template auto-fills.
Get-Content .github\pull_request_template.md
Select-String -Path README.md -Pattern "How to run"

##Checklist
Tests added or updated
README updated if behavior changed
