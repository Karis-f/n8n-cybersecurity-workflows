# 🛡️ n8n Cybersecurity Workflows

Production-ready n8n workflows untuk **Incident Response (IR)** dan **Phishing Analysis** yang terintegrasi dengan AI (Claude Sonnet 4).

## 📋 Daftar Workflow

| Workflow | Status | Deskripsi |
|----------|--------|-----------|
| [🚨 Incident Response](workflows/incident-response/) | ✅ Production | Auto-triage, containment, AI forensic analysis |
| [📧 Phishing Analysis](workflows/phishing-analysis/) | 🚧 In Progress | Email analysis, IOC enrichment, auto-block |

## ⚡ Quick Start

### Prasyarat
- n8n ≥ 1.60
- Docker & Docker Compose (recommended)
- Anthropic API key
- Slack webhook URL (opsional)

### Instalasi

```bash
# 1. Clone repo
git clone https://github.com/your-username/n8n-cybersecurity-workflows.git
cd n8n-cybersecurity-workflows

# 2. Setup environment
cp docker/.env.example docker/.env
# Edit docker/.env — isi API keys

# 3. Jalankan n8n
cd docker
docker-compose up -d

# 4. Import workflow
# Buka http://localhost:5678
# Workflows → Import from File → pilih workflows/incident-response/ir-production.json
