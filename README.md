# ⚔️ Netdata System Monitor

<div align="center">

![Netdata](https://img.shields.io/badge/Netdata-00AB44?style=for-the-badge&logo=netdata&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

> *"Even the weakest signal... Netdata will find it."* 🗡️

<img src="https://media.giphy.com/media/AXorq7GFST89O/giphy.gif" width="280"/>

</div>

---

## 🏯 Mission

Deploy **Netdata** via Docker and monitor your system in **real-time** — CPU, RAM, Network & more — straight from your browser.

---

## ⚡ Quick Setup

```bash
# 1. Install Docker
sudo apt update && sudo apt install -y docker.io
sudo systemctl enable --now docker
sudo usermod -aG docker $USER && newgrp docker

# 2. Launch Netdata
docker run -d --name=netdata -p 19999:19999 netdata/netdata

# 3. Verify
docker ps

# 4. Open Dashboard 🌐
# http://localhost:19999
```

---

## 📊 Dashboard Preview

| File | What it shows |
|------|--------------|
| `netdata_dashboard.png` | Full metrics view |
| `netdata_metrics_local.png` | Local system stats |
| `netdata_container.png` | Docker container status |
| `nodes.png` | Connected nodes |

---

## 🛠️ Useful Commands

```bash
docker stop netdata      # 😴 Sleep
docker start netdata     # ⚡ Wake up
docker logs -f netdata   # 📜 View logs
docker rm -f netdata     # 💀 Destroy
```

---

<div align="center">

*Made with 🍜 and way too much caffeine*

</div>
