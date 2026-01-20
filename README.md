# Nouveaux Paradigmes - TD3/TD4

Auteur : Carette Robin  
Depot : https://github.com/CaretteRobin/nouveaux-paradigmes-TD3-4.git

## Contenu
- `docker-compose.yml` : Directus + base de donnees
- `.env.example` : exemple de configuration (copier en `.env`)
- `data/` : fichiers CSV d'import
- `TD3-directus-rendu.pdf` : rendu TD3
- `TD4-graphql-rendu.pdf` : rendu TD4
- captures ecran a la racine (preuves)

## Demarrage rapide
```bash
cp .env.example .env
docker compose up -d
```

Acces Directus : `http://localhost:8055`

## Import CSV (ordre conseille)
1. specialite
2. structure
3. moyen_paiement
4. motif_visite
5. praticien
6. praticien2motif
7. praticien2moyen
