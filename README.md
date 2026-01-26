## 👋 Welcome to fider 🚀

Open-source feedback and feature request platform

## 📋 Description

Open-source feedback and feature request platform

## 🚀 Services

- **fider**: fider/fider:latest

### Infrastructure Components

- **fider-db**: Postgres database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/fider/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/fider" ~/.local/srv/docker/fider
cd ~/.local/srv/docker/fider
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install fider
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:3003

## 📂 Volumes

- `./rootfs/data/fider` - Data storage
- `./rootfs/config/fider` - Data storage
- `./rootfs/data/db/postgres/fider` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f fider
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
