# ReturnReview — Complete Backup Repository

This repository is the disaster-recovery mirror for **Rishikeshsanin/ReturnReview**.

It is designed to preserve much more than a simple source-code copy:

- `project/` — complete tracked working-tree snapshot from ReturnReview `main`
- `archives/ReturnReview-full-history.bundle` — Git bundle containing complete accessible Git history/refs
- `releases/` — GitHub Release metadata and downloadable release assets, including CV checkpoints
- `metadata/` — source repository, branch, tag, issue, PR, workflow and run metadata
- `SHA256SUMS.txt` — integrity hashes
- `RESTORE.md` — restoration instructions
- `BACKUP_STATUS.md` — exact source SHA and known backup gaps

## Security

**Secrets are never backed up to GitHub.** Provider API keys, database credentials, tokens, and resolved environment values are intentionally excluded.

## Railway/PostgreSQL

The source project used Railway for the web/API/PostgreSQL runtime. The Railway trial expired on 2026-10-25, stopping the services. A fresh PostgreSQL logical dump must be added after the database service is restored. Until then, the application/schema/model/deployment material is backed up here, while the latest live database rows remain dependent on Railway's retained volume.

## Source of truth

Primary project: https://github.com/Rishikeshsanin/ReturnReview

This backup should be refreshed whenever the primary project changes materially.
