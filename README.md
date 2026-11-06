# netauto-lab

A network automation CI/CD portfolio project. A virtual multi-site network
(built in GNS3) is managed as code and validated by a pipeline.

## Topology

See [docs/topology.md](docs/topology.md).

- 2 WAN routers (IOSv), one per site, linked to each other
- 4 core switches (NX-OSv), 2 per site, in a square between the sites

## Repository layout

| Folder | Purpose |
|---|---|
| `inventory/` | Device inventory and variables |
| `playbooks/` | Ansible playbooks |
| `templates/` | Config templates (Jinja2) |
| `tests/` | Validation and pre/post checks |
| `docs/` | Diagrams and notes |

## Roadmap

- [x] Phase 1: Foundations (git, platform, first IOSv and NX-OSv boot)
- [ ] Phase 2: Source of truth (NetBox/Nautobot)
- [ ] Phase 3: Ansible config management and Vault
- [ ] Phase 4: Linting and testing (pyATS / Batfish)
- [ ] Phase 5: CI/CD pipeline
- [ ] Phase 6: Fabric and IPNs

## Notes

Cisco images are licensed and are not included in this repo.
