# Task 7 – Monitor System Resources Using Netdata

## Commands to Complete the Task

### 1️⃣ Install Docker (Linux)
```bash
sudo apt update
sudo apt install -y docker.io
sudo systemctl enable --now docker
sudo usermod -aG docker $USER && newgrp docker
docker --version

## Run Netadata Container
docker run -d --name=netdata -p 19999:19999 netdata/netdata

## Verify Netdata is running
docker ps

## Access Netdata Dashboard 
http://localhost:19999
