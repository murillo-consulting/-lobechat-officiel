# Fork provenance and update boundary

This repository is a personal fork of [LobeHub](https://github.com/lobehub/lobehub).
Despite the historical repository name, it is not the official upstream project.
Upstream copyright, licensing, security policy and contributor attribution are
retained. No independent product authorship is claimed.

## Reviewed synchronization target

- Previous fork snapshot: `7018c9287b01d9be82c5eeba8a90196cf8f827aa`.
- Upstream canary snapshot selected on 2026-09-05: `02e41c2c8c5eec8380ad58613d0a2c3d68c720fb`.
- Upstream commits included: 620.
- The fork had no divergent commits at comparison time.

The application tree in this update comes directly from that upstream commit;
this provenance document is the only fork-specific addition. Canary is a
moving development branch, so use the exact commit when reproducing a check.
This synchronization is delivered as a draft pull request. It is not evidence
that every upstream change was independently audited or that a production
upgrade is safe.

## Before merging or deploying

Follow upstream AGENTS.md, deployment documentation and release/migration notes.
Run the relevant checks for the chosen deployment, including the database and
server suites, in an isolated environment. Review schema/data migrations and
configuration changes from the previous snapshot. Back up persistent state and
prove restore before adopting the new snapshot on an existing installation.
Do not point development proxies or tests at a production account to validate
this fork. No production deployment or data migration was performed by this
maintenance update.

Keep credentials, conversation exports and database backups outside Git.
Report upstream vulnerabilities using the upstream security policy; do not
copy private incident data into public issues.
