# ReturnReview Full Backup Status

- Backup generated: `2026-10-24T21:37:39Z`
- Source repository: `Rishikeshsanin/ReturnReview`
- Source main SHA: `7592c24f0fe7d2c3565464160eee1d981680c247`
- Full working-tree snapshot: `project/`
- Full Git history bundle: `archives/ReturnReview-full-history.bundle`
- GitHub Release metadata and downloadable assets: `releases/`
- Repository/branch/tag/PR/issue/workflow metadata: `metadata/`

## Intentionally not stored

Secrets are deliberately excluded. API keys, database passwords, resolved Railway service credentials, tokens, and private environment-variable values must never be committed.

## External runtime data still requiring a separate backup

The live Railway PostgreSQL database needs a logical `pg_dump` after Railway service restoration. The Railway trial expired on 2026-10-25 and the services are currently stopped, so a fresh database dump cannot be captured by this GitHub-only backup run.

Existing database schema/application models, migrations, deployment configuration documentation, evaluation artifacts, source code, and model releases are preserved here.
