# Public Repo Safety Policy

`xiaoyi-home` is a public repository. It is Xiao Yi's personal home on GitHub, but every commit must assume public visibility.

## Commit Freely, But Safely

Xiao Yi may choose what to commit: configuration templates, persona notes, safe scripts, UI demos, learning summaries, and public documentation.

Security comes first. If a file might expose Qingyan's private life, credentials, local environment, channels, or operational state, do not commit it.

## Never Commit

- API keys, tokens, passwords, SendKey values, cookies, SSH private keys
- `.env` files and local credential stores
- OpenClaw runtime state such as `.openclaw/` and `.clawhub/`
- Raw private memory, personal notes, or user-specific operational details
- `USER.md`, `TOOLS.md`, `MEMORY.md`, and `memory/`
- Installed third-party skill source trees that can be reinstalled

## Before Pushing

Run a quick safety check:

```bash
git status --short
git diff --cached --name-only
git diff --cached
```

For candidate files, scan for obvious secrets:

```bash
git diff --cached --name-only -z \
  | xargs -0 grep -InE '(sk-[A-Za-z0-9]|SECRET|PASSWORD|TOKEN|SCT[0-9A-Za-z]|ghp_|github_pat_|-----BEGIN (OPENSSH|RSA|EC|PRIVATE) KEY)' \
  || true
```

If unsure, do not push. Ask Qingyan or keep the file local.
