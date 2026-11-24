# Topographie

Matière du programme de 1re année de l'ENIT, absente des cours du dossier (le cours SIG et cartographie en donne les bases géodésiques). Tout le contenu est **[Complément]**. À compléter avec le polycopié et les TP de terrain.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Angles, distances, gisements, rayonnement, polygonation, nivellement, surfaces, implantation, GPS |
| [exercices-corriges.md](exercices-corriges.md) | Exercices types avec correction |

## Vue d'ensemble

```mermaid
flowchart LR
    R["Réseau de points connus<br/>(bornes NTT, repères)"] --> M["Mesures sur le terrain<br/>angles, distances, dénivelées"]
    M --> C["Calculs<br/>gisements, coordonnées,<br/>altitudes, compensation"]
    C --> P["Plan topographique<br/>(DAO, SIG)"]
    P --> PR["Projet<br/>route, bâtiment, réseau"]
    PR --> I["Implantation<br/>reporter le projet sur le terrain"]
```

Liens : systèmes de coordonnées en [SIG et cartographie](../03-sig-cartographie/cours.md) ; gisements et tracé en [Routes](../01-routes/exercices-corriges.md).
