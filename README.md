# 📊 Monitoring Homelab

Система мониторинга на базе **Zabbix + Grafana**, развёрнутая с помощью **Docker и Ansible**.

> **Автор**: [Maxim Rygalov](https://github.com/maximrygalov)

---

## 🛠️ Состав
- **Zabbix Server + Web UI** — http://localhost:8080 (`Admin` / `zabbix`)
- **Zabbix Agent** — мониторинг WSL2-хоста
- **PostgreSQL** — база данных Zabbix
- **Grafana** — http://localhost:3000 (`admin` / `admin`)

---

## ▶️ Как запустить

```bash
git clone https://github.com/maximrygalov/monitoring-homelab.git
cd monitoring-homelab
ansible-playbook setup-monitoring.yml
```

> Требуется: Docker, Docker Compose, Ansible (проверено в WSL2).
