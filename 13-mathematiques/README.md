# Mathématiques et analyse numérique

Matière du programme de 1re année de l'ENIT, absente des cours du dossier. Tout le contenu est **[Complément]**, centré sur les outils dont l'ingénieur génie civil se sert dans les autres matières.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Algèbre linéaire, analyse, équations différentielles, probabilités et statistiques, méthodes numériques |
| [exercices-corriges.md](exercices-corriges.md) | Exercices types avec correction |

## Où sert chaque outil ?

```mermaid
flowchart LR
    AL["Algèbre linéaire<br/>systèmes, valeurs propres"] --> RDM["RDM, structures<br/>(méthode des déplacements)"]
    AL --> MMC["MMC<br/>contraintes principales"]
    AN["Analyse<br/>dérivées, intégrales"] --> RDM
    ED["Équations différentielles"] --> RDM2["Déformée des poutres<br/>EI y'' = M"]
    ED --> DYN["Vibrations, pendule"]
    PS["Probabilités, statistiques<br/>Gumbel, période de retour"] --> HYD["Hydrologie"]
    NUM["Méthodes numériques<br/>Newton, Simpson, Euler"] --> TOUT["Calculs sur ordinateur<br/>(programmation)"]
```
