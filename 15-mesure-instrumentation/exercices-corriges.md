# Exercices corrigés de mesure et instrumentation

[← Retour au sommaire](README.md)

**[Complément]** : exercices types, à vérifier avec l'enseignant.

---

## Exercice 1. Série de mesures

On mesure cinq fois le diamètre d'une éprouvette de béton (mm) : 159,8 ; 160,2 ; 160,0 ; 159,9 ; 160,1. Donner le résultat avec une incertitude élargie (k = 2).

### Correction

- Moyenne : x̄ = 800,0 / 5 = **160,0 mm**.
- Écarts : −0,2 ; 0,2 ; 0 ; −0,1 ; 0,1 → somme des carrés = 0,10.
- s = √(0,10 / 4) = 0,158 mm ; u = s / √5 = 0,071 mm ; U = 2u = 0,14 mm.

**D = 160,0 ± 0,1 mm** (k = 2).

---

## Exercice 2. Propagation des incertitudes

Une éprouvette cylindrique de diamètre D = 160,0 ± 0,1 mm se rompt sous F = 603 ± 3 kN. Calculer la contrainte de rupture et son incertitude (méthode majorante).

### Correction

- S = πD²/4 = π × 160² / 4 = 20 106 mm².
- σ = F / S = 603 000 / 20 106 = **29,99 MPa**.
- Δσ/σ = ΔF/F + 2 ΔD/D = 3/603 + 2 × 0,1/160 = 0,00498 + 0,00125 = 0,0062.
- Δσ = 0,0062 × 30,0 = 0,19 MPa.

**σ = 30,0 ± 0,2 MPa.**

---

## Exercice 3. Lecture d'un pied à coulisse

Pied à coulisse au 1/20 (0,05 mm). Le zéro du vernier est entre 41 et 42 mm sur la règle ; le 9ᵉ trait du vernier coïncide avec un trait de la règle. Quelle est la mesure ?

### Correction

41 + 9 × 0,05 = **41,45 mm**.

---

## Exercice 4. Jauge de déformation

Une jauge (K = 2,1) est montée en quart de pont alimenté sous E = 5 V, sur une barre d'acier (E_acier = 210 000 MPa). On lit V_s = 1,05 mV. Calculer la déformation et la contrainte.

### Correction

- ε = 4 V_s / (E K) = 4 × 1,05·10⁻³ / (5 × 2,1) = 4,0·10⁻⁴ = **400 µm/m**.
- σ = E_acier ε = 210 000 × 4·10⁻⁴ = **84 MPa**.

---

## Exercice 5. Convertisseur et échantillonnage

Un capteur de déplacement LVDT donne 0 à 10 V pour 0 à 50 mm. Il est relié à un CAN 16 bits de plage 0-10 V. On veut suivre une vibration de 20 Hz.

1. Quelle est la sensibilité du capteur ?
2. Quelle est la plus petite variation de déplacement détectable par le CAN ?
3. Quelle fréquence d'échantillonnage minimale choisir ?

### Correction

1. S = 10 V / 50 mm = **0,2 V/mm**.
2. q = 10 / 2¹⁶ = 0,153 mV, soit 0,153·10⁻³ / 0,2 = **0,76 µm**.
3. Shannon : fₑ > 2 × 20 = 40 Hz ; en pratique **200 Hz** environ (10 × f_max).

---

## Exercice 6. Étalonnage d'un capteur de force

On applique des charges connues x (kN) et on lit la sortie y (mV) :

| x (kN) | 0 | 10 | 20 | 30 | 40 |
| --- | --- | --- | --- | --- | --- |
| y (mV) | 0,1 | 2,0 | 4,1 | 5,9 | 8,0 |

Trouver la droite d'étalonnage, puis la force correspondant à y = 6,6 mV.

### Correction

- n = 5 ; Σx = 100 ; Σy = 20,1 ; Σx² = 3 000 ; Σxy = 0 + 20 + 82 + 177 + 320 = 599.
- a = (5 × 599 − 100 × 20,1) / (5 × 3 000 − 100²) = (2 995 − 2 010) / 5 000 = **0,197 mV/kN**.
- b = 20,1/5 − 0,197 × 20 = 4,02 − 3,94 = **0,08 mV**.
- x = (6,6 − 0,08) / 0,197 = **33,1 kN**.
