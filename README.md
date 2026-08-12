# health-imaging-platform

Multi-tenant medical imaging ingestion, de-identification, and cohort/research
platform on AWS. See `/docs/architecture/` for design docs and ADRs.

## Repository layout

| Folder | Contents |
|---|---|
| `/infra` | AWS CDK stacks — DynamoDB, S3, OpenSearch, Step Functions, IAM, networking |
| `/services` | Backend services — ingestion, validation, de-identification, consent, billing webhooks |
| `/ui` | Frontend portal (patient/tenant-facing and internal ops views) |
| `/shared` | Shared libraries — types, clients, utilities used across services and infra |
| `/scripts` | One-off and operational scripts (data migrations, backfills, local dev setup) |
| `/docs` | Architecture docs, ADRs, runbooks |
| `/.github` | CI/CD workflows, PR template, CODEOWNERS |

## Getting started

1. Clone the repo and run `pre-commit install` (see `.pre-commit-config.yaml`).
2. See `/docs/README.md` for links to architecture docs.
3. See each folder's own `README.md` for folder-specific setup notes.

## Contributing

All changes go through a pull request — direct pushes to `main` are blocked.
See `.github/PULL_REQUEST_TEMPLATE.md` for the PR checklist and `.github/CODEOWNERS`
for who reviews what.
