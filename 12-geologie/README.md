# Géologie de l'ingénieur

Matière du programme de 1re année de l'ENIT, absente des cours du dossier. Tout le contenu est **[Complément]**. À compléter avec le polycopié de l'enseignant.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Structure de la Terre, minéraux, roches, temps géologiques, déformations, cartes géologiques, eaux souterraines, risques, géologie de la Tunisie |
| [exercices-corriges.md](exercices-corriges.md) | Questions et exercices types avec correction |

## Vue d'ensemble

```mermaid
flowchart LR
    T["La Terre<br/>structure, tectonique"] --> M["Minéraux"]
    M --> R["Roches<br/>magmatiques, sédimentaires,<br/>métamorphiques"]
    R --> D["Déformations<br/>plis, failles"]
    D --> C["Carte et coupe géologiques"]
    R --> H["Eaux souterraines<br/>nappes"]
    C --> G["Projet de génie civil<br/>fondations, tunnels, carrières,<br/>barrages, tracé routier"]
    H --> G
    D --> RI["Risques<br/>séismes, glissements"]
    RI --> G
```

Suite logique : [mécanique des sols](../07-mecanique-des-sols/cours.md).
