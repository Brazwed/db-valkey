# db-valkey

Valkey 8 Docker container pré-configurado. Fork comunitário do Redis, compatível com a API Redis.

## Uso rápido

```bash
git clone https://github.com/Brazwed/db-valkey.git
cd db-valkey
docker compose up -d
```

## Conexão padrão

```
Host:     localhost
Porta:    6380
Senha:    valkey_dev_2026

redis-cli -h localhost -p 6380 -a valkey_dev_2026
```

## Configuração

Edite `.env` (criado automaticamente de `.env.example`):

```env
VK_PORT=6380
VK_PASS=valkey_dev_2026
VK_MAXMEMORY=512mb
```

## Parte do Database Toolkit

Este repositório pode ser usado standalone ou junto com outros bancos via [Database](https://github.com/Brazwed/Database).
