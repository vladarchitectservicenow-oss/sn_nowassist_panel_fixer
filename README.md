# sn_nowassist_panel_fixer

## Architecture
```mermaid
graph TD
    SN[ServiceNow] -->|REST| sn_nowassist_panel_fixer
    sn_nowassist_panel_fixer -->|Store| DB[Tables]
    sn_nowassist_panel_fixer -->|Generate| Report[Reports]
```
## Quick Start
```bash
git clone https://github.com/vladarchitectservicenow-oss/sn_nowassist_panel_fixer.git
cd sn_nowassist_panel_fixer && python3 src/cli.py --help
```
## ROI
| Approach | Hours/Year | Cost |
|----------|-----------|------|
| Manual | 40 | $3,400 |
| With sn_nowassist_panel_fixer | 5 | $425 |
| **Savings** | **35h** | **$2,975 (87%)** |
## API Reference
`GET /api/now/table/incident` — incidents
## Security
- HTTPS, credentials via env vars, GDPR compliant
## Troubleshooting
| Issue | Fix |
|-------|-----|
| Timeout | `--timeout 60` |
| 401 | Check credentials |
## License
Copyright (C) 2026 Vladimir Kapustin | AGPL-3.0

