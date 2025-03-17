# Tyk Docker Configuration Files

This repository contains example configuration files for deploying Tyk components using Docker in a **single-node setup**.  
These files are intended to help you understand component connectivity and configuration when running Tyk locally.

## Components Covered
- Tyk Gateway
- Tyk Dashboard
- Tyk Pump

---

## Files Included
| File Name              | Description                                  |
|------------------------|----------------------------------------------|
| `tyk.conf`             | Tyk Gateway configuration file               |
| `tyk_analytics.conf`   | Tyk Dashboard configuration file             |
| `pump.conf`            | Tyk Pump configuration file                  |

---

## Default Ports Matrix
| Component      | Default Port | Description                    |
|----------------|--------------|--------------------------------|
| Tyk Gateway    | 8080         | Public API traffic             |
| Tyk Dashboard  | 3000         | Admin UI                       |
| Tyk Pump       | 8083         | Metrics pump (optional access) |
| MongoDB        | 27017        | Database                      |
| Redis          | 6379         | Cache / session store          |

---

## Installation Sequence
It's important to start services in this order to avoid connection issues:
1. **MongoDB/PostgreSQL** & **Redis**
2. **Tyk Dashboard**
3. **Tyk Pump**
4. **Tyk Gateway**


---

## Raw File Links (Direct Access)
- [tyk.conf](https://raw.githubusercontent.com/rahmatlatif/tyk-docker-configs/main/tyk.conf)
- [tyk_analytics.conf](https://raw.githubusercontent.com/rahmatlatif/tyk-docker-configs/main/tyk_analytics.conf)
- [pump.conf](https://raw.githubusercontent.com/rahmatlatif/tyk-docker-configs/main/pump.conf)

---

## License
This repository is for educational/demo purposes.
