# db-valkey

Valkey 8 Docker container pre-configured. Community Redis fork, API compatible.

## Quick Start

```bash
git clone https://github.com/Brazwed/db-valkey.git
cd db-valkey
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

Edit `.env` (created automatically from `.env.example`):

```env
VK_PORT=6380
VK_PASS=valkey_dev_2026
VK_MAXMEMORY=512mb
```

## Part of Database Toolkit

This repo can be used standalone or with other databases via [Database Toolkit](https://github.com/Brazwed/Database).
