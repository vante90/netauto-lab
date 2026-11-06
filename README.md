# WAN CI/CD Automation

A network automation CI/CD WAN project. A virtual multi-site WAN
(built in GNS3) is managed as code and validated by a pipeline.

## Topology

See [docs/topology.md](docs/topology.md): 10 IOSv WAN routers (A1, A2, B1,
B2, C1, C2, D1, D2, E1, E2) connected by 15 links.

## Repository layout

| Folder | Purpose |
|---|---|
| `inventory/` | Device inventory and variables |
| `playbooks/` | Ansible playbooks |
| `templates/` | Config templates (Jinja2) |
| `tests/` | Validation and pre/post checks |
| `docs/` | Diagrams and notes |

## Roadmap

- [ ] Phase 1: Foundations (git, platform, first router boot)
- [ ] Phase 2: Source of truth (NetBox/Nautobot)
- [ ] Phase 3: Ansible config management and Vault
- [ ] Phase 4: Linting and testing (pyATS / Batfish)
- [ ] Phase 5: CI/CD pipeline

## Notes

Cisco images are licensed and are not included in this repo.
