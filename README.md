# rada-netdata

Instance Netdata auto-hébergée, derrière Traefik, déployée sur le Raspberry via GitHub Actions.

## Fichiers

- `docker-compose.yml` : définition du service netdata + labels Traefik.
- `.env` : configuration locale (non versionnée), basé sur `.env.example`
- `.github/workflows/deploy.yml` : pipeline de déploiement sur le Raspberry

## Déploiement

1. Cloner le repo sur le Raspberry dans `/home/rada/apps/rada-netdata`.
2. Copier `.env.example` en `.env` et l'adapter.
3. Lancer une première fois :

```bash
docker compose up -d
```

