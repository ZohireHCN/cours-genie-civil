# Exercices corrigés de topographie

[← Retour au sommaire](README.md)

Exercices types. Calculs vérifiés numériquement. Angles en grades.

---

## Exercice 1. Gisement et distance

A (1 000,00 ; 2 000,00) et B (1 250,00 ; 1 800,00). Calculer D_AB, G_AB et G_BA.

### Correction

ΔX = +250,00 ; ΔY = −200,00 : quadrant **Sud-Est**.

$$D = \sqrt{250^2 + 200^2} = 320{,}16\ \text{m} \qquad g = \arctan\frac{250}{200} = 57{,}0447\ \text{gr}$$

$$G_{AB} = 200 - 57{,}0447 = 142{,}9553\ \text{gr} \qquad G_{BA} = 342{,}9553\ \text{gr}$$

---

## Exercice 2. Rayonnement

Depuis S (500,00 ; 500,00), on mesure vers P : G = 60,0000 gr et D = 150,00 m. Coordonnées de P ?

### Correction

60 gr = 54°.

$$X_P = 500 + 150\sin60\ \text{gr} = 500 + 121{,}35 = 621{,}35 \qquad Y_P = 500 + 150\cos60\ \text{gr} = 500 + 88{,}17 = 588{,}17$$

---

## Exercice 3. Fermeture angulaire

Quadrilatère fermé ABCD, angles intérieurs mesurés : 98,1240 – 102,4570 – 95,3320 – 104,0910 gr. Tolérance 0,0060 gr. Compenser.

### Correction

Somme théorique : (4 − 2) × 200 = 400 gr. Somme mesurée : 400,0040 gr.

f = +0,0040 gr < 0,0060 : **acceptable**. Correction : −0,0040 / 4 = −0,0010 gr par angle.

| Angle | Mesuré | Compensé |
| --- | --- | --- |
| A | 98,1240 | 98,1230 |
| B | 102,4570 | 102,4560 |
| C | 95,3320 | 95,3310 |
| D | 104,0910 | 104,0900 |
| Somme | 400,0040 | **400,0000** |

---

## Exercice 4. Cheminement de nivellement fermé

Départ et arrivée sur le repère R (Z = 100,000 m). Tolérance : 10 mm.

| Station | Point AR | Lecture AR | Point AV | Lecture AV |
| --- | --- | --- | --- | --- |
| 1 | R | 1,524 | P1 | 0,862 |
| 2 | P1 | 1,210 | P2 | 2,035 |
| 3 | P2 | 1,705 | R | 1,548 |

### Correction

| Station | ΔH = AR − AV | Correction | ΔH compensée | Point | Z (m) |
| --- | --- | --- | --- | --- | --- |
| | | | | R | 100,000 |
| 1 | +0,662 | +0,002 | +0,664 | P1 | 100,664 |
| 2 | −0,825 | +0,002 | −0,823 | P2 | 99,841 |
| 3 | +0,157 | +0,002 | +0,159 | R | **100,000** ✔ |

- ΣAR − ΣAV = 4,439 − 4,445 = −0,006 m : la fermeture vaut **−6 mm** < 10 mm, acceptable.
- On répartit +6 mm sur 3 stations : +2 mm chacune.

---

## Exercice 5. Nivellement trigonométrique

Station en A (hi = 1,50 m), prisme en B (hv = 1,70 m). Dh = 200,00 m, angle zénithal V = 97,5000 gr. Z_A = 52,30 m. Z_B ?

### Correction

$$\Delta H = \frac{D_h}{\tan V} + h_i - h_v = \frac{200}{\tan 97{,}5\ \text{gr}} + 1{,}50 - 1{,}70 = 7{,}858 - 0{,}200 = 7{,}658\ \text{m}$$

V < 100 gr : la visée monte, B est plus haut. **Z_B = 59,96 m**.

---

## Exercice 6. Surface d'une parcelle (Gauss)

Sommets : 1 (0 ; 0), 2 (40 ; 0), 3 (50 ; 30), 4 (10 ; 35). Surface ?

### Correction

| i | Xi | Yi | Xi·Yi+1 | Xi+1·Yi |
| --- | --- | --- | --- | --- |
| 1 | 0 | 0 | 0 × 0 = 0 | 40 × 0 = 0 |
| 2 | 40 | 0 | 40 × 30 = 1 200 | 50 × 0 = 0 |
| 3 | 50 | 30 | 50 × 35 = 1 750 | 10 × 30 = 300 |
| 4 | 10 | 35 | 10 × 0 = 0 | 0 × 35 = 0 |
| Somme | | | 2 950 | 300 |

$$S = \frac{|2950 - 300|}{2} = 1\,325\ \text{m}^2$$

---

## Exercice 7. Implantation d'un point

Station S (500,00 ; 500,00), référence R (500,00 ; 800,00). On doit implanter le coin de bâtiment P (621,35 ; 588,17). Quel angle tourner depuis la référence, et quelle distance reporter ?

### Correction

- G_SR : ΔX = 0, ΔY = +300 : G = **0,0000 gr** (plein Nord). On vise R et on affiche 0 sur le cercle.
- G_SP : c'est le point de l'exercice 2 : G = **60,0000 gr**, D = **150,00 m**.
- On tourne la lunette jusqu'à lire 60,0000 gr, on reporte 150,00 m (distance horizontale) et on plante le piquet. Contrôle depuis une autre station ou par une mesure de distance entre deux points implantés.
