# /.github

Repository governance and CI/CD configuration.

**What goes here:**
- `CODEOWNERS` — required reviewers per path
- `PULL_REQUEST_TEMPLATE.md` — PR checklist (tests, secrets, docs, cdk-nag)
- `workflows/` — GitHub Actions CI/CD pipelines (add as they're built:
  lint/test on PR, cdk-nag checks, deploy pipelines per environment)
- `ISSUE_TEMPLATE/` — bug report / feature request templates (add as needed)

Changes here affect how *every* PR in the repo is reviewed and gated, so this
folder itself requires platform-lead review (see `CODEOWNERS`).
