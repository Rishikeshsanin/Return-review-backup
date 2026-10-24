# ReturnReview Full Backup Status

- Backup generated: 
- Source repository: 
- Source main SHA: 
- Full working-tree snapshot: 
- Full Git history bundle: 
- GitHub Release metadata and downloadable assets: 
- Repository/branch/tag/PR/issue/workflow metadata: 

## Intentionally not stored

Secrets are deliberately excluded. API keys, database passwords, resolved Railway service credentials, tokens, and private environment-variable values must never be committed.

## External runtime data still requiring a separate backup

The live Railway PostgreSQL database needs a logical  after Railway service restoration. The Railway trial expired on 2026-10-25 and the services are currently stopped, so a fresh database dump cannot be captured by this GitHub-only backup run.

Existing database schema/application models, migrations, deployment configuration documentation, evaluation artifacts, source code, and model releases are preserved here.
