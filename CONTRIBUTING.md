# Contributing to google-dorks

Thank you for helping grow this database! Every dork added helps security
researchers and defenders worldwide find and fix real exposures.

---

## ✅ What We Accept

- New dork patterns targeting real, documented security misconfigurations
- New category files for technologies not yet covered
- Updates to outdated dorks in existing files
- README or documentation improvements

## ❌ What We Do NOT Accept

- Dorks targeting specific named individuals or private entities
- Dorks with no realistic security research application
- Duplicates of patterns already in existing files
- Any content intended to facilitate unauthorized access

---

## 📁 File Naming Convention

google-dorks-for-[technology].txt

Place the file in the most relevant category folder:

| Folder | Use for |
|--------|---------|
| `cloud/` | Cloud provider misconfigs |
| `credentials/` | Keys, secrets, env files |
| `services/` | SaaS platforms and APIs |
| `devops/` | Pipelines, containers, IaC |
| `vulnerabilities/` | Attack surface patterns |
| `monitoring/` | Dashboards and observability |
| `cms/` | Content management systems |
| `web-server/` | Web infrastructure |
| `recon/` | Passive intelligence gathering |
| `files/` | Leaked documents |

---

## 📝 File Format

Google Dorks for [Technology]
Purpose: [One sentence — what these dorks help find]
Added by: [your GitHub username]
[dork 1]

[dork 2]

[dork 3]


Rules:
- One dork per line
- No trailing whitespace
- `#` comments only in the header block
- Keep all dorks relevant to the file's named technology

---

## 🔀 Pull Request Process

1. Fork this repository
2. Create a branch: `git checkout -b add/google-dorks-for-[technology]`
3. Add or edit files following the format above
4. Update `all-google-dorks.txt` with any new dorks you added
5. Commit using the format below
6. Open a PR against the `main` branch

---

## 💬 Commit Message Format

add: google-dorks-for-[technology].txt — [short description]

fix: google-dorks-for-[technology].txt — [what was fixed]

refactor: [description of structural change]

docs: [description of documentation update]

Examples:

add: google-dorks-for-docker.txt — exposed compose files and registry credentials

fix: google-dorks-for-env-files.txt — add Next.js and Vite .env patterns

docs: README.md — add category index table


---

## ⚖️ Legal & Ethical Requirements

By submitting a pull request you confirm that:
- Your contribution is intended for lawful, authorized security research only
- You have not tested these dorks against systems you don't own or have permission to test
- Your contribution complies with applicable laws in your jurisdiction

---

## 🙏 Credits & Attribution

This is a community fork of
[Proviesec/google-dorks](https://github.com/Proviesec/google-dorks).
All original dork content is the work of Proviesec and the original contributors.

New dorks, folder structure, and documentation in this fork were added by
[souhailbakioui](https://github.com/souhailbakioui).

All contributors to this fork are credited via Git commit history.