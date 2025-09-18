# LKvitai.MES – Microservices for Blinds Manufacturing

This GitHub Organization contains all repositories related to **LKvitai.MES** – a microservice-based Manufacturing Execution System for blinds production.  
It covers order intake, warehouse management, shopfloor operations, reporting, and integrations with external systems (Agnum, Avea).

---

## 🚀 Core Services
- [**lkvitai-warehouse-service**](https://github.com/lkvitai/lkvitai-warehouse-service) – Warehouse management (stock, reservations, movements, batches).
- [**lkvitai-shopfloor-service**](https://github.com/lkvitai/lkvitai-shopfloor-service) – Shopfloor task execution (cutting, assembling, QC).
- [**lkvitai-orders-service**](https://github.com/lkvitai/lkvitai-orders-service) – Order management and processing.
- [**lkvitai-auth-service**](https://github.com/lkvitai/lkvitai-auth-service) – Authentication & user management.

---

## 🛠 Infrastructure & Standards
- [**lkvitai-mes-devstack**](https://github.com/lkvitai/lkvitai-mes-devstack) – Local dev environment (Docker Compose, Traefik, Node-RED, MQTT, SQL).
- [**lkvitai-mes-infra**](https://github.com/lkvitai/lkvitai-mes-infra) – Deployment scripts (Proxmox, VPS, WireGuard, Caddy, Ansible/PowerShell).
- [**lkvitai-mes-standards**](https://github.com/lkvitai/lkvitai-mes-standards) – Shared configs: `.editorconfig`, `Directory.Build.props`, reusable GitHub Actions.

---

## 📦 Shared Libraries
- [**Lkvitai.MES.Contracts**](https://github.com/lkvitai/Lkvitai.MES.Contracts) – DTOs, events, enums shared across services (NuGet).
- [**Lkvitai.MES.SharedKernel**](https://github.com/lkvitai/Lkvitai.MES.SharedKernel) – Common abstractions (Result, Guard, DomainEvents).
- [**Lkvitai.MES.Clients**](https://github.com/lkvitai/Lkvitai.MES.Clients) – Typed API clients (generated via NSwag).

---

## 💻 Frontend & Prototypes
- [**lkvitai-mvc-portal**](https://github.com/lkvitai/lkvitai-mvc-portal) – Operator/Manager web portal (ASP.NET MVC + Bootstrap).
- [**lkvitai-rete-prototypes**](https://github.com/lkvitai/lkvitai-rete-prototypes) – Experimental Node-RED / Rete.js UI for tech rules and formulas.

---

## 📖 Naming Conventions

| Layer             | Convention / Example |
|-------------------|-----------------------|
| **Organization**  | `lkvitai` |
| **Repos (services)** | `lkvitai-<context>-service` → `lkvitai-warehouse-service` |
| **Repos (infra)** | `lkvitai-mes-<purpose>` → `lkvitai-mes-devstack` |
| **Docker images** | `ghcr.io/lkvitai/<name>:<tag>` → `ghcr.io/lkvitai/warehouse-service:1.0.0` |
| **.NET namespaces** | `Lkvitai.MES.<Context>` → `Lkvitai.MES.Warehouse` |
| **NuGet packages** | `Lkvitai.MES.<Context>` → `Lkvitai.MES.Contracts` |
| **Events (MQTT)** | `<context>.<entity>.<action>` → `warehouse.item.received` |

---

## 🔗 Useful Links
- 📚 [Confluence Documentation](https://confluence.company.local/display/LKVITAI)  
- 📦 [Azure DevOps (builds, artifacts)](https://dev.azure.com/lkvitai/)  
- 📊 [Grafana Monitoring](https://grafana.lkvitai.local)  
- 🐳 [Docker Hub / GHCR Packages](https://github.com/orgs/lkvitai/packages)

---

Maintained by **Denis Bykovas**  
