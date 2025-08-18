# 🏠 My Homelab Setup

This repo documents my **homelab running on Fedora 42** with **Docker**.  
The Objective was to create a self hosted homelab that was capable of running multiple services and that could serve my needs and use cases.
Each service runs in its own `docker-compose.yml` file inside its own folder.

---

## 🚀 Services

- **Netdata** → System monitoring
- **Portainer** → Docker container management
- **Homarr** → Dashboard for quick access
- **n8n** → Workflow automation
- **Jellyfin** → Media server
- **Radarr** → Movies
- **Sonarr** → TV shows
- **Prowlarr** → Indexer manager
- **qBittorrent** → Torrent client
- **FreshRSS** → RSS reader
- **FiveFilters Full-Text RSS** → Convert feeds to full articles

---

## 📦 How to Run
1. Install Docker & Docker Compose.
2. Clone this repo.
3. Navigate to a service folder (e.g. `jellyfin/`).
4. Copy `.env.example` → `.env` and set your values.
5. Start with:
   ```bash
   docker compose up -d
