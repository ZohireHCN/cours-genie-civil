# Mécanique des fluides et hydraulique

Matière du programme de 1re année de l'ENIT, absente des cours du dossier. Tout le contenu est **[Complément]**. À compléter avec le polycopié de l'enseignant.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Propriétés des fluides, hydrostatique, continuité, Bernoulli, pertes de charge, écoulements à surface libre |
| [exercices-corriges.md](exercices-corriges.md) | Exercices types avec correction |

## Vue d'ensemble

```mermaid
flowchart LR
    P["Propriétés<br/>ρ, viscosité μ, ν"] --> H["Hydrostatique<br/>fluide au repos<br/>p = p0 + ρgh, Archimède"]
    P --> D["Hydrodynamique<br/>continuité Q = V·S<br/>Bernoulli"]
    D --> C["En charge (conduites)<br/>Reynolds, pertes de charge"]
    D --> L["À surface libre (canaux, dalots)<br/>Manning-Strickler, Froude"]
    C --> A["AEP, réseaux sous pression"]
    L --> O["Assainissement, ouvrages<br/>hydrauliques routiers"]
```

Le débit de projet calculé en [Hydrologie](../02-hydrologie/cours.md) sert ici à dimensionner l'ouvrage (exercice 7).
