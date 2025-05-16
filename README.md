# Blockcast Beacon Guide Using VPS  
_For setups where Docker is already installed_

This guide will walk you through running a Blockcast BEACON node on your VPS using Docker and Docker Compose.

---

## 📥 Step 1: Clone the Docker Compose Repo

```bash
git clone https://github.com/Blockcast/beacon-docker-compose.git
cd beacon-docker-compose

```
## Step 2: Start the BEACON Node
To start the BEACON node in the background, run:

```bash
docker compose up -d

```

## Step 3: Generate Your Hardware ID & Challenge Key
Run this command to generate your Hardware ID and Challenge Key:

```bash
docker compose exec blockcastd blockcastd init

```

## Step 4: Copy the part that has 'HTTP', paste it into your browser, and it will automatically display the node key
