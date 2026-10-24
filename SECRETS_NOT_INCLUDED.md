# Secrets Are Not Part of This Backup

This repository is intended to be a comprehensive project backup, but **not a secret vault**.

Deliberately excluded:
- Gemini API keys
- Railway tokens
- PostgreSQL passwords/resolved DATABASE_URL values
- Roboflow API keys
- GitHub tokens/secrets
- any other private provider credentials

Rotate/recreate secrets when restoring the project.
