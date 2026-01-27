# Nouveaux Paradigmes - TD3/TD4

Auteur : Carette Robin  
Depot : https://github.com/CaretteRobin/nouveaux-paradigmes-TD3-4.git

## Contenu
- `docker-compose.yml` : Directus + base de donnees
- `.env.example` : exemple de configuration (copier en `.env`)
- `data/` : fichiers CSV d'import
- `TD3-directus-rendu.pdf` + `TD3-directus-rendu.md` : rendu TD3
- `TD4-graphql-rendu.pdf` + `TD4-graphql-rendu.md` : rendu TD4
- `RENDU.md` : note de rendu (contexte + lien git)
- `screens/` : captures ecran (preuves)
- `bruno/TD4-graphql/` : collection Bruno (requetes et mutations TD4)

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

## TD4 - Execution des requetes GraphQL (Bruno)
Le dossier `bruno/TD4-graphql/` contient toutes les requetes du TD4 (Q1 a Q10, tests d'auth, mutations).

1) Lancer Directus si besoin
```bash
docker compose up -d
```

2) Importer la collection Bruno
- Ouvrir Bruno
- Importer le dossier `bruno/TD4-graphql/`

3) Configurer l'environnement
- Ouvrir l'environnement `Local`
- Renseigner :
  - `baseUrl` : `http://localhost:8055`
  - `token` : token Directus (role `td4_reader` ou admin)

4) Executer les requetes
- Lancer les requetes `Q1` a `Q10`
- Tester les acces avec `Auth-*`
- Executer les mutations `M1` a `M8`
