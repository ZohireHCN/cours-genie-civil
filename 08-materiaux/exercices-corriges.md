# Exercices corrigés de matériaux

[← Retour au sommaire](README.md)

Exercices types. Calculs vérifiés numériquement.

---

## Exercice 1. Masses volumiques

On remplit un récipient de 1 L avec un gravier sec : 1 500 g. On verse 1 000 g du même gravier dans une éprouvette contenant de l'eau : le niveau monte de 377 cm³. Calculer les masses volumiques apparente et absolue, la porosité du tas.

### Correction

- Apparente : 1 500 g / 1 000 cm³ = **1,50 t/m³**.
- Absolue : 1 000 / 377 = **2,65 t/m³** (calcaire ou silice).
- Porosité du tas (vides entre grains) : p = 1 − 1,50 / 2,65 = **0,43**, soit 43 % de vides. C'est ce vide que le sable puis la pâte de ciment doivent remplir dans un béton.

---

## Exercice 2. Module de finesse d'un sable

Refus cumulés : 5 mm : 2 % ; 2,5 mm : 12 % ; 1,25 mm : 30 % ; 0,63 mm : 52 % ; 0,315 mm : 75 % ; 0,16 mm : 92 %. Calculer MF et conclure.

### Correction

$$MF = \frac{2 + 12 + 30 + 52 + 75 + 92}{100} = 2{,}63$$

Entre 2,2 et 2,8 : **bon sable à béton**. Un MF < 1,8 (sable trop fin) demanderait plus d'eau ; un MF > 3,2 (trop grossier) donnerait un béton peu maniable.

---

## Exercice 3. Los Angeles

5 000 g de gravillons ; après l'essai, 1 250 g passent au tamis de 1,6 mm. LA ? Utilisable en couche de roulement (LA < 30 exigé) ?

### Correction

LA = 100 × 1 250 / 5 000 = **25** < 30 : **oui**.

---

## Exercice 4. Rapport E/C par Bolomey

On veut fc28 = 25 MPa avec un ciment de classe vraie σ′c = 42,5 MPa et G = 0,5. Le dosage en ciment est de 350 kg/m³. Quel C/E, quelle quantité d'eau ?

### Correction

$$\frac{C}{E} = \frac{f_{c28}}{G\,\sigma'_c} + 0{,}5 = \frac{25}{0{,}5\times42{,}5} + 0{,}5 = 1{,}68$$

E = 350 / 1,68 = **209 L/m³**, soit E/C = 0,60.

Si l'ouvrier ajoute 30 L d'eau par m³ sur chantier : C/E = 350 / 239 = 1,46 et fc28 = 0,5 × 42,5 × (1,464 − 0,5) = **20,5 MPa** : une perte de près de 20 %.

---

## Exercice 5. Essais de résistance

1. Une éprouvette de béton 16 × 32 cm casse sous 520 kN. Résistance ?
2. Une barre HA12 atteint sa limite élastique sous 56,5 kN. Nuance de l'acier ?

### Correction

1. Section : π × 80² = 20 106 mm². fc = 520 000 / 20 106 = **25,9 MPa**.
2. Section : π × 6² = 113,1 mm². fe = 56 500 / 113,1 = **500 MPa** : **FeE500**.

---

## Exercice 6. Choisir les matériaux

Pour chaque ouvrage, proposer le ciment, le type de béton ou le liant.

| Ouvrage | Choix |
| --- | --- |
| Fondation dans un sol gypseux (sud tunisien) | ? |
| Dalle coulée en été à 40 °C | ? |
| Couche de roulement d'une route à fort trafic | ? |
| Traitement d'un sol argileux humide de plateforme | ? |
| Poteaux d'un immeuble en bord de mer | ? |

### Correction

| Ouvrage | Choix |
| --- | --- |
| Sol gypseux (sulfates) | Ciment **HRS** (résistant aux sulfates), E/C faible |
| Bétonnage par forte chaleur | **Retardateur** de prise, bétonner tôt le matin, cure soignée |
| Couche de roulement | **Béton bitumineux** avec bitume dur 40/50 et granulats LA et MDE faibles |
| Sol argileux humide | Traitement à la **chaux** |
| Bord de mer | Béton compact (E/C ≤ 0,5), **enrobage** augmenté (4 à 5 cm), ciment adapté au milieu marin |
