# SHA-1 & Objects

## Git internal structure — commit identification and integrity

Git uses SHA-1 hashes for commit identification.

- **SHA-1** is a cryptographic hash function
- It generates a unique digital fingerprint for each file/commit
- Ensures file integrity and serves as a reference (e.g., in `git revert [SHA]`)

Hashes are visible in `git log` or on GitHub pages and are used across many Git commands.

\newpage
