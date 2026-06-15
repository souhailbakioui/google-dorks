# 🔍 Google Dorks — Security Research Database

[![License](https://img.shields.io/badge/license-MIT-red.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)
[![Stars](https://img.shields.io/github/stars/souhailbakioui/google-dorks?style=social)](https://github.com/souhailbakioui/google-dorks/stargazers)
[![Forks](https://img.shields.io/github/forks/souhailbakioui/google-dorks?style=social)](https://github.com/souhailbakioui/google-dorks/forks)
[![Forked from](https://img.shields.io/badge/forked%20from-Proviesec%2Fgoogle--dorks-blue?style=flat)](https://github.com/Proviesec/google-dorks)

> A structured, community-maintained database of Google Dorks for defensive
> security research, bug bounty programs, and authorized penetration testing.
> Originally compiled by [Proviesec](https://github.com/Proviesec).

---


Explore the Google Dorks database through the web interface:

Website: [https://dorksearch-pro.vercel.app](https://dorksearch-pro.vercel.app/)


## ⚠️ Legal Disclaimer

This repository is intended **exclusively** for:
- Authorized penetration testing
- Bug bounty programs within defined scope
- Defensive auditing of systems you own or have explicit permission to test

**Using these dorks against systems without authorization is illegal.**
The maintainers accept no responsibility for misuse. See [SECURITY.md](SECURITY.md).

---

## 📁 Repository Structure

```txt
google-dorks/

├── cloud/              # AWS, GCP, Azure, Firebase, Kubernetes
├── credentials/        # API keys, .env files, git secrets, JS secrets
├── services/           # Stripe, Slack, OpenAI, Twilio, SendGrid, Discord
├── devops/             # Docker, Terraform, Jenkins, GitHub Actions, CI/CD
├── vulnerabilities/    # SQLi, XSS, open redirect, Swagger
├── monitoring/         # Grafana, Kibana, Elasticsearch
├── cms/                # WordPress, Joomla, Magento, Typo3
├── web-server/         # Nginx, Apache, login panels, frameworks
├── recon/              # Bug bounty, company recon, stats
├── files/              # Excel, PDF, presentation, backup leaks
├── finding-username-passwords/
├── technology/
├── all-google-dorks.txt      # Master list — all dorks combined
├── best-google-dorks.txt     # Curated top picks
└── google-dorks-best-log.txt # Changelog
```


---

## 🔎 What is a Google Dork?

A Google Dork is an advanced search query using Google's built-in operators
to surface information that is publicly indexed but not intended to be
easily discoverable — such as exposed credentials, open admin panels,
misconfigured servers, and leaked files.

---

## 🧰 Core Search Operators

| Operator | Description | Example |
|----------|-------------|---------|
| `intext:` | Search for keywords in page body | `intext:"db_password"` |
| `intitle:` | Search in page title | `intitle:"index of"` |
| `inurl:` | Search within URLs | `inurl:"/admin/login"` |
| `site:` | Restrict to a domain | `site:*.gov` |
| `filetype:` | Filter by file extension | `filetype:env` |
| `ext:` | Alias for filetype | `ext:sql` |
| `before:` / `after:` | Date range filter | `after:2024-01-01` |
| `"..."` | Exact phrase match | `"secret_key"` |
| `-` | Exclude term | `-demo -test` |
| `OR` / `\|` | Either term | `site:s3.amazonaws.com \| site:storage.googleapis.com` |

---

## 📂 Category Index

### ☁️ Cloud
| File | Description |
|------|-------------|
| `cloud/google-dorks-for-aws-s3.txt` | Exposed S3 buckets and IAM credentials |
| `cloud/google-dorks-for-azure.txt` | Azure storage and config leaks |
| `cloud/google-dorks-for-gcp.txt` | Google Cloud Platform misconfigs |
| `cloud/google-dorks-for-firebase.txt` | Firebase database exposure |
| `cloud/google-dorks-for-kubernetes.txt` | K8s dashboards and kubeconfig leaks |
| `cloud/google-dorks-for-cloud-platforms.txt` | General cloud platform patterns |

### 🔑 Credentials
| File | Description |
|------|-------------|
| `credentials/google-dorks-for-env-files.txt` | Exposed .env files |
| `credentials/google-dorks-for-api-keys.txt` | Generic API key patterns |
| `credentials/google-dorks-for-js-secrets.txt` | Secrets hardcoded in JS |
| `credentials/google-dorks-for-git-files.txt` | .git directory and config exposure |
| `credentials/google-dorks-for-database-files.txt` | SQL dumps and DB credentials |

### 🛠️ DevOps
| File | Description |
|------|-------------|
| `devops/google-dorks-for-docker.txt` | Docker Compose and registry exposure |
| `devops/google-dorks-for-terraform.txt` | tfstate files and cloud secrets |
| `devops/google-dorks-for-jenkins.txt` | Jenkins dashboards and Script Console |
| `devops/google-dorks-for-ci-cd.txt` | General CI/CD pipeline leaks |
| `devops/google-dorks-for-github-actions.txt` | GitHub Actions secrets and workflows |
| `devops/google-dorks-for-backups.txt` | Exposed backup files and archives |

### 🌐 Services
| File | Description |
|------|-------------|
| `services/google-dorks-for-openai.txt` | OpenAI API key exposure |
| `services/google-dorks-for-anthropic.txt` | Anthropic API key exposure |
| `services/google-dorks-for-stripe.txt` | Stripe secret key leaks |
| `services/google-dorks-for-sendgrid.txt` | SendGrid API key exposure |
| `services/google-dorks-for-mailgun.txt` | Mailgun credential leaks |
| `services/google-dorks-for-twilio.txt` | Twilio auth token exposure |
| `services/google-dorks-for-slack.txt` | Slack webhook and token leaks |
| `services/google-dorks-for-discord.txt` | Discord token and webhook leaks |
| `services/google-dorks-for-mongodb.txt` | MongoDB connection string exposure |

### 🐛 Vulnerabilities
| File | Description |
|------|-------------|
| `vulnerabilities/google-dorks-for-sql-injection.txt` | SQLi entry points |
| `vulnerabilities/google-dorks-for-xss.txt` | XSS vulnerable parameters |
| `vulnerabilities/google-dorks-for-open-redirect.txt` | Open redirect patterns |
| `vulnerabilities/google-dorks-for-swagger.txt` | Exposed Swagger/OpenAPI docs |

### 📊 Monitoring
| File | Description |
|------|-------------|
| `monitoring/google-dorks-for-grafana.txt` | Exposed Grafana dashboards |
| `monitoring/google-dorks-for-kibana.txt` | Open Kibana instances |
| `monitoring/google-dorks-for-elasticsearch.txt` | Unauthenticated ES clusters |
| `monitoring/google-dorks-for-monitoring.txt` | General monitoring panel exposure |

### 🖥️ CMS
| File | Description |
|------|-------------|
| `cms/google-dorks-for-wordpress.txt` | wp-config, user enum, debug logs |
| `cms/google-dorks-for-joomla.txt` | Joomla config and admin panels |
| `cms/google-dorks-for-magento.txt` | Magento admin and config leaks |
| `cms/google-dorks-for-typo3.txt` | Typo3 installation exposure |

### 🌍 Web Server
| File | Description |
|------|-------------|
| `web-server/google-dorks-for-webserver.txt` | Web server misconfigs |
| `web-server/google-dorks-for-login.txt` | Exposed login panels |
| `web-server/google-dorks-for-conf.txt` | Config file exposure |
| `web-server/google-dorks-for-frameworks.txt` | Framework-specific patterns |

### 🕵️ Recon
| File | Description |
|------|-------------|
| `recon/google-dorks-for-bug-bounty-programs.txt` | Bug bounty scope recon |
| `recon/google-dorks-for-companys.txt` | Company asset discovery |
| `recon/google-dorks-for-stats.txt` | Exposed statistics and analytics |
| `recon/google-dorks-for-wikipedia.txt` | Wikipedia-based recon patterns |

### 📎 Files
| File | Description |
|------|-------------|
| `files/google-dorks-for-excel-files.txt` | Exposed Excel spreadsheets |
| `files/google-dorks-for-presentations.txt` | Leaked presentation files |

---

## 🛡️ Preventing Google Dorking Against Your Site

1. **Audit yourself first** — run these dorks against your own domain regularly
2. **Use `robots.txt`** — block sensitive paths from crawlers
3. **Set `X-Robots-Tag: noindex`** headers on admin/staging environments
4. **Remove sensitive files** from public web roots entirely
5. **Use Google Search Console** to de-index accidentally exposed pages
6. **Never commit secrets** to public repositories

Example `robots.txt` protection:

User-agent: *

Disallow: /admin/

Disallow: /backup/

Disallow: /.env

Disallow: /wp-config.php

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add new dorks,
fix existing ones, or propose new categories.

---

## 🔗 Resources

- [Exploit-DB Google Hacking Database](https://www.exploit-db.com/google-hacking-database)
- [OSINT Framework](https://osintframework.com)
- [Google Advanced Search](https://www.google.com/advanced_search)
- [Proviesec Medium Articles](https://proviesec.medium.com/)

---

## 📜 License

MIT License — see [LICENSE](LICENSE) for full text.

## 👥 Credits & Attribution

Original database compiled and maintained by
[Proviesec](https://github.com/Proviesec) —
[github.com/Proviesec/google-dorks](https://github.com/Proviesec/google-dorks).

This repository is a **community fork** that extends the original with:
- Reorganized folder structure by threat category
- New dork files: Docker, Terraform, Jenkins, Elasticsearch, WordPress, API Keys
- Added `CONTRIBUTING.md`, `SECURITY.md`, and `LICENSE`
- Improved `README.md` with full category index and operator reference

All original content remains the work of Proviesec and contributors.
New additions by [souhailbakioui](https://github.com/souhailbakioui).
