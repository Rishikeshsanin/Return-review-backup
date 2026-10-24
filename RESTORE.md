# ReturnReview Restore Guide

## Restore the source tree
Copy the contents of `project/` into a clean repository/worktree.

## Restore full Git history
```bash
git clone archives/ReturnReview-full-history.bundle ReturnReview-restored
cd ReturnReview-restored
git checkout main
```

## Restore CV models
The approved model binaries and release manifests are under `releases/`. The production release is `cv-lightweight-1`.

## Restore hosted runtime
Recreate/restore the documented Railway services only from the ReturnReview project documentation. Do not copy secrets from documentation; use fresh environment secrets.

## Restore database
After a PostgreSQL dump is added to this repository or another secure backup location:
```bash
pg_restore --clean --if-exists --no-owner --dbname="<target-url>" <dump-file>
```

Never commit plaintext database URLs, API keys, OAuth tokens, or provider secrets.
