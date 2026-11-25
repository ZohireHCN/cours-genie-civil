# Géologie de l'ingénieur

Matière de 1re année (ESSAT Gabès, cours du samedi). Les chapitres 1 à 4 suivent **mes notes de cours manuscrites** ; la suite est un **[Complément]** construit sur le programme usuel, à remplacer au fur et à mesure du cours.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Ch. 1-2 : la Terre, rôle du sol de fondation. Ch. 3 : grands ensembles structuraux (continents, océans, marges, ceintures orogéniques, mers). Ch. 4 : minéraux et cristallographie. Suite [Complément] : roches, temps géologiques, déformations, cartes, eaux souterraines, risques, Tunisie |
| [exercices-corriges.md](exercices-corriges.md) | Questions et exercices types avec correction (exercices 7 à 9 sur mes chapitres) |
| [images/marges-continentales.svg](images/marges-continentales.svg) | Coupe marge passive / marge active |

## Vue d'ensemble

```mermaid
flowchart LR
    T["Ch. 1-2<br/>La Terre, sol de fondation"] --> S["Ch. 3<br/>Grands ensembles structuraux"]
    S --> M["Ch. 4<br/>Minéraux, cristallographie"]
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
