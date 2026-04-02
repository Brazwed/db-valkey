# db-valkey

Valkey 8 Docker container pre-configured. Community Redis fork.

## Option 1: Use with Database Toolkit (Recommended)

```bash
git clone --recurse-submodules https://github.com/Brazwed/Database.git
cd Database
sudo ./setup.sh install valkey
```

## Option 2: Standalone with Docker Compose

```bash
git clone https://github.com/Brazwed/db-valkey.git
cd db-valkey
cp .env.example .env
docker compose up -d
```

## Default Connection

```
Host:     localhost
Port:     6380
Pass:     valkey_dev_2026

redis-cli -h localhost -p 6380 -a valkey_dev_2026
```

## Configuration

Edit `.env`:

```env
VK_PORT=6380
VK_PASS=valkey_dev_2026
VK_MAXMEMORY=512mb
```

## Part of Database Toolkit

https://github.com/Brazwed/Database
