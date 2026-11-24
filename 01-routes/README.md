# Routes

Cours complet de Routes, basé sur le cours « COURS ROUTE 2GCV » et les « EXERCICES ROUTES 2GCV ». Les passages marqués **[Complément]** ne viennent pas du cours.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Les 9 chapitres : définitions, formules, exemples chiffrés |
| [formulaire.md](formulaire.md) | Toutes les formules sur une page |
| [exercices-corriges.md](exercices-corriges.md) | Exercices types avec correction détaillée |

## Vue d'ensemble

Un projet routier suit toujours le même chemin : on fixe la vitesse, on en déduit la géométrie, puis on dimensionne la chaussée avec le trafic et le sol.

```mermaid
flowchart TD
    V[Vitesse de référence Vr<br/>catégorie de route] --> TP[Tracé en plan<br/>alignements, cercles, clothoïdes]
    V --> DS[Distances de sécurité<br/>freinage, arrêt, dépassement]
    TP --> R[Rayons minimaux<br/>RHm, RHN, RHd, RHnd]
    TP --> PL[Profil en long<br/>déclivités, rayons verticaux]
    DS --> PL
    PL --> PT[Profils en travers]
    PT --> TER[Terrassements<br/>cubatures déblais / remblais]
    TRA[Trafic poids lourds<br/>trafic cumulé TC] --> CH[Structure de chaussée]
    SOL[Sol support<br/>classe S0 à S4, CBR] --> CH
    TER --> CH
```

## Plan du cours

1. Marché routier et étapes d'un chantier
2. Tracé routier : terminologie, tracé en plan, rayons, surlargeur
3. Raccordements circulaires
4. Paramètres fondamentaux : distances de freinage, d'arrêt, de dépassement
5. Trafic routier : trafic cumulé, classes, capacité
6. Clothoïde et dévers
7. Profil en long et profil en travers
8. Structure de chaussée et dimensionnement
9. Terrassements [Complément]
