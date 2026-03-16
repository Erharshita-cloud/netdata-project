# ⚔️ Task 7 — Netdata System Monitor

<div align="center">

![Netdata](https://img.shields.io/badge/Netdata-00AB44?style=for-the-badge&logo=netdata&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00FF99&center=true&vCenter=true&width=500&lines=Monitoring+System+Resources...;Netdata+on+Docker+%F0%9F%90%B3;Real-time+Metrics+%E2%9A%A1;Port+19999+is+LIVE+%F0%9F%9F%A2" alt="Typing SVG" />

> *"Even the weakest signal... Netdata will find it."* 🗡️

<!-- 
  💡 TIP: Upload an anime GIF to your repo (e.g. assets/anime.gif)
  Then replace the line below with:
  <img src="./assets/anime.gif" width="280"/>
-->
<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="700"/>

</div>

---

## 🏯 Mission

Deploy **Netdata** via Docker and monitor your system in **real-time** — CPU, RAM, Network & more — straight from your browser.

---

## ⚡ Quick Setup

```bash
# 1️⃣ Install Docker
sudo apt update && sudo apt install -y docker.io
sudo systemctl enable --now docker
sudo usermod -aG docker $USER && newgrp docker

# 2️⃣ Launch Netdata
docker run -d --name=netdata -p 19999:19999 netdata/netdata

# 3️⃣ Verify
docker ps

# 4️⃣ Open Dashboard 🌐
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
<img src="https://user-images.githubusercontent.com/74038190/212284158-e840e285-664b-44d7-b79b-e264b5e54825.gif" width="400"/>

*Made with 🍜 and way too much caffeine*
</div>
