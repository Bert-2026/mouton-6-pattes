# mouton-6-pattes

Recherche de parcelles et de biens en Deux-Sèvres à partir d'une description : cadastre, photos aériennes IGN, zonage PLU, bâtiments, ventes DVF et risques.

**Ouvrir l'application :** https://bert-2026.github.io/mouton-6-pattes/

## Ce que fait l'application

- Lit une description (« au moins 2 bâtiments habitables avec dépendances à rénover, sur 2 500 m² minimum… ») et remplit les critères.
- Cherche dans une commune, un cercle ou une zone dessinée sur la carte, parmi **toutes** les parcelles cadastrales, vendues ou non.
- Filtres : surface (m²), eau, bois, haies, accès, forme, pente, nombre de bâtiments et bâtiments habitables, année de construction, zonage PLU (U, 1AU, 2AU, A, N, codes précis), ventes passées, zones inondables, PPR, espaces boisés classés, emplacements réservés, abords de monuments historiques.
- Résultats sur photo aérienne, liens Géoportail, Google Satellite, Géoportail de l'Urbanisme, Géorisques et recherche d'annonces, export CSV.

## Données (publiques, sans clé)

| Donnée | Service |
|---|---|
| Communes | geo.api.gouv.fr |
| Parcelles, zonage PLU, prescriptions, servitudes | API Carto (IGN) |
| Bâtiments (usage, logements, date) | BD TOPO, Géoplateforme IGN (WFS) |
| Photos aériennes, Plan IGN, cadastre, altitude | Géoplateforme IGN |
| Eau, bois, haies, routes | OpenStreetMap (Overpass) |
| Ventes passées | DVF : Cerema DVF+, Micro-API DVF ou data.gouv.fr |
| Risques | Géorisques |

L'application ne garde aucune donnée sur un serveur : tout se passe dans le navigateur. Ce n'est ni un état des risques officiel ni un certificat d'urbanisme ; vérifiez toujours auprès de la mairie et sur les sites officiels.
