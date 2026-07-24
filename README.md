# Homelab Structure

This repository contains the infrastructure and services for my self-hosted homelab and personal AI assistant (Jarvis).

## Directory Layout

```text
homelab/
├── compose/
├── configs/
├── data/
├── backups/
├── docs/
├── infrastructure/
├── services/
└── scripts/
```

### compose/

Docker Compose files for deploying services.

Examples:

- homepage.yml
- ollama.yml
- postgres.yml
- monitoring.yml

---

### configs/

Application configuration files.

Examples:

- Caddy
- Grafana
- Prometheus
- Homepage

---

### data/

Persistent application data (volumes).

Examples:

- PostgreSQL databases
- Ollama models
- Grafana data
- Qdrant collections

This directory is **not** tracked by Git.

---

### backups/

Application and database backups.

Examples:

- PostgreSQL dumps
- Configuration backups
- Scheduled snapshots

---

### docs/

Project documentation.

Examples:

- Architecture
- Network setup
- Docker notes
- Setup guides
- TODOs

---

### infrastructure/

Infrastructure-related configuration.

Examples:

- Kubernetes manifests
- Helm charts
- Terraform
- Ansible
- GitOps configuration

---

### services/

One directory per deployed service.

Example:

```text
services/
├── homepage/
├── ollama/
├── postgres/
├── qdrant/
└── jarvis/
```

Each service may contain:

- compose.yml
- README.md
- configuration
- scripts

---

### scripts/

Automation scripts.

Examples:

- backup.sh
- restore.sh
- deploy.sh
- update.sh

---

## Git

The repository tracks:

- Infrastructure
- Docker Compose
- Configuration
- Documentation
- Scripts

The following are **not** committed:

- Application data
- Backups
- Secrets
- Environment files
