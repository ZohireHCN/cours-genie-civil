# Matériaux de construction

Matière du programme de 1re année de l'ENIT, absente des cours du dossier. Tout le contenu est **[Complément]**. À compléter avec le polycopié et les TP de l'enseignant.

## Fichiers

| Fichier | Contenu |
| --- | --- |
| [cours.md](cours.md) | Propriétés, granulats, liants, béton, mortiers, aciers, liants hydrocarbonés, autres matériaux |
| [exercices-corriges.md](exercices-corriges.md) | Exercices types avec correction |

## Vue d'ensemble

```mermaid
flowchart TD
    M["Matériaux de construction"] --> MIN["Minéraux"]
    M --> MET["Métaux"]
    M --> ORG["Organiques"]
    MIN --> GR["Granulats<br/>sable, gravier"]
    MIN --> LI["Liants hydrauliques<br/>chaux, ciment"]
    MIN --> CE["Terre cuite<br/>briques, tuiles"]
    GR --> BE["Béton, mortier"]
    LI --> BE
    MET --> AC["Aciers pour béton armé<br/>profilés"]
    AC --> BA["Béton armé"]
    BE --> BA
    ORG --> BI["Bitumes<br/>enrobés routiers"]
    ORG --> BO["Bois"]
    GR --> BI
```
