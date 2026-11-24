# Exercices corrigés de géologie

[← Retour au sommaire](README.md)

---

## Exercice 1. Identifier une roche

On dispose de quatre échantillons :

1. roche grise, compacte, fait effervescence à l'acide ;
2. roche blanche, se raye à l'ongle, pas d'effervescence ;
3. roche à grains visibles roses, blancs et noirs, raye le verre ;
4. roche grise, se délite dans l'eau en pâte collante.

### Correction

1. **Calcaire** (calcite → effervescence).
2. **Gypse** (dureté 2).
3. **Granite** (feldspath rose, quartz blanc, mica noir ; roche magmatique plutonique, texture grenue).
4. **Argile** ou marne (plastique dans l'eau).

---

## Exercice 2. Chronologie relative

Sur une coupe, on observe de bas en haut : des grès (A), des argiles (B), des calcaires (C). Une faille F décale A, B et C. Des alluvions (D) horizontales recouvrent le tout sans être décalées. Ordre des événements ?

### Correction

```mermaid
flowchart LR
    A["1. Dépôt des grès A"] --> B["2. Argiles B"] --> C["3. Calcaires C"] --> F["4. Faille F<br/>(recoupe A, B, C)"] --> E["5. Érosion"] --> D["6. Alluvions D<br/>(non faillées)"]
```

Principes utilisés : superposition (A, B, C), recoupement (F postérieure à C), D non décalée donc postérieure à F. La faille n'a pas rejoué depuis le dépôt de D : indice qu'elle est peut-être inactive (à confirmer).

---

## Exercice 3. Épaisseur d'une couche

Sur un plateau horizontal, une couche de calcaire affleure sur une largeur de 50 m, mesurée perpendiculairement à sa direction. Son pendage est de 30°. Épaisseur réelle ?

### Correction

$$e = l\sin p = 50\times\sin30° = 25\ \text{m}$$

---

## Exercice 4. Lire un pendage

Une couche est notée N45°E, 20° NW. La décrire.

### Correction

Les horizontales de la couche sont orientées à 45° du Nord vers l'Est (direction NE-SW). La couche plonge de 20° vers le Nord-Ouest, perpendiculairement à sa direction.

---

## Exercice 5. Choix de site

Un projet de route près de Gabès doit choisir entre trois tracés :

- tracé 1 : traverse une sebkha sur 2 km ;
- tracé 2 : longe le pied d'un versant marneux, avec des traces de glissements anciens ;
- tracé 3 : plus long de 1,5 km, sur un plateau à croûte calcaire.

### Correction

| Tracé | Problèmes | Solutions possibles et coût |
| --- | --- | --- |
| 1 | Sol très compressible, salé (agressif pour le béton), nappe affleurante, inondable | Remblai important, géotextile, ciment HRS, drainage : coûteux, risques de tassement |
| 2 | Instabilité de talus réactivée par les déblais et la pluie | Drainage, soutènements, surveillance : risque à long terme |
| 3 | Plus long, terrassements dans la croûte (rippage ou explosifs) | Bonne portance, matériaux réutilisables |

Le **tracé 3** est le plus sûr. Le surcoût de longueur est souvent compensé par l'économie sur les fondations de chaussée et l'entretien. La décision finale demande une reconnaissance géotechnique (sondages, essais) et une comparaison chiffrée.

---

## Exercice 6. Questions de cours

1. Pourquoi le gypse pose-t-il problème en génie civil ?
2. Différence entre nappe libre et nappe captive ?
3. Pourquoi les argiles et marnes sont-elles associées aux glissements ?

### Correction

1. Il est **soluble** (cavités, effondrements, tassements quand l'eau circule) et ses sulfates **attaquent le béton** (gonflement, fissuration) : il faut des ciments résistants aux sulfates.
2. Nappe libre : surface à la pression atmosphérique, sous une zone non saturée. Nappe captive : entre deux couches imperméables, sous pression ; dans un forage, l'eau remonte au-dessus du toit de l'aquifère.
3. Elles sont peu perméables (l'eau y fait monter la pression interstitielle), leur résistance chute quand elles se saturent (σ′ = σ − u diminue, voir la [mécanique des sols](../07-mecanique-des-sols/cours.md)) et elles ont souvent des plans de glissement anciens.
