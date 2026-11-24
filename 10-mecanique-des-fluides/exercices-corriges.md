# Exercices corrigés de mécanique des fluides

[← Retour au sommaire](README.md)

Exercices types. Calculs vérifiés numériquement. g = 9,81 m/s², ρ = 1 000 kg/m³.

---

## Exercice 1. Pression hydrostatique

Pression relative au fond d'un château d'eau de 10 m de hauteur d'eau ? En bar ?

### Correction

p = ρ g h = 1 000 × 9,81 × 10 = **98 100 Pa** ≈ **0,98 bar**. Un étage de 3 m demande environ 0,3 bar : c'est pour cela que les réservoirs sont placés en hauteur.

---

## Exercice 2. Force sur un mur de bassin

Un bassin a une paroi verticale de 4 m de large ; l'eau a 3 m de profondeur. Force de l'eau et point d'application ?

### Correction

$$F = \frac{\rho g\,b\,h^2}{2} = \frac{1000\times9{,}81\times4\times3^2}{2} = 176\,580\ \text{N} \approx 177\ \text{kN}$$

Appliquée à h/3 = **1 m** au-dessus du fond. Moment au pied du mur : 177 × 1 = 177 kN·m, à reprendre par le mur et sa fondation (voir la [RDM](../06-rdm/cours.md)).

---

## Exercice 3. Poussée d'Archimède

Un cube de bois de 0,5 m de côté (ρ = 600 kg/m³) flotte dans l'eau. Enfoncement ?

### Correction

Poids : 600 × 9,81 × 0,125 = 735,8 N. À l'équilibre, poussée = poids : 1 000 × 9,81 × (0,5 × 0,5 × e) = 735,8, d'où **e = 0,30 m**.

Plus simplement : e / 0,5 = 600 / 1 000, donc e = 0,30 m (60 % de la hauteur est immergée).

---

## Exercice 4. Continuité

Une conduite de 200 mm de diamètre, où l'eau circule à 1,5 m/s, se réduit à 100 mm. Débit et vitesse dans la petite conduite ?

### Correction

$$Q = V_1 S_1 = 1{,}5\times\frac{\pi\times0{,}2^2}{4} = 0{,}0471\ \text{m}^3/\text{s} = 47{,}1\ \text{L/s}$$

$$V_2 = V_1\left(\frac{D_1}{D_2}\right)^2 = 1{,}5\times4 = 6{,}0\ \text{m/s}$$

---

## Exercice 5. Vidange d'un réservoir (Torricelli)

Un réservoir se vide par un orifice de 5 cm de diamètre situé 5 m sous la surface. Vitesse théorique et débit réel (Cd = 0,62) ?

### Correction

$$V = \sqrt{2gh} = \sqrt{2\times9{,}81\times5} = 9{,}90\ \text{m/s}$$

$$Q = C_d\,S\,V = 0{,}62\times\pi\times0{,}025^2\times9{,}90 = 0{,}0121\ \text{m}^3/\text{s} = 12{,}1\ \text{L/s}$$

---

## Exercice 6. Perte de charge dans une conduite

La conduite de 200 mm de l'exercice 4 mesure 500 m, λ = 0,02. Reynolds et perte de charge ?

### Correction

$$Re = \frac{1{,}5\times0{,}2}{10^{-6}} = 3\times10^5 \quad\text{: turbulent}$$

$$\Delta H = 0{,}02\times\frac{500}{0{,}2}\times\frac{1{,}5^2}{2\times9{,}81} = 50\times0{,}1147 = 5{,}73\ \text{m}$$

Il faut 5,73 m de charge (≈ 0,56 bar) pour faire passer ce débit sur 500 m.

---

## Exercice 7. Capacité d'un dalot (lien avec l'hydrologie)

L'examen d'[hydrologie](../02-hydrologie/exercices-corriges.md) donne un débit de projet Q₅₀ ≈ 29,7 m³/s. On propose un dalot en béton (K = 70) de cellules 3 m de large, avec une hauteur d'eau admissible de 1,5 m, pente 0,5 %. Combien de cellules ? Régime ?

### Correction

Pour une cellule : S = 3 × 1,5 = 4,5 m² ; P = 3 + 2 × 1,5 = 6 m ; Rh = 0,75 m.

$$Q_1 = 70\times4{,}5\times0{,}75^{2/3}\times\sqrt{0{,}005} = 70\times4{,}5\times0{,}825\times0{,}0707 = 18{,}4\ \text{m}^3/\text{s}$$

Une cellule ne suffit pas (18,4 < 29,7). **Deux cellules** : 36,8 m³/s > 29,7 ✔ (en pratique, on garde une revanche au-dessus de l'eau).

Vitesse : V = 18,4 / 4,5 = 4,09 m/s ; $Fr = 4{,}09 / \sqrt{9{,}81\times1{,}5} = 1{,}07$ : **légèrement torrentiel**. À la sortie, il faut protéger le lit (enrochements, bassin de dissipation) contre l'érosion.

```mermaid
flowchart LR
    H["Hydrologie<br/>Q50 = 29,7 m³/s"] --> M["Manning-Strickler<br/>1 cellule 3 × 1,5 m : 18,4 m³/s"]
    M --> N["2 cellules : 36,8 m³/s ✔"]
    N --> F["Fr = 1,07 : protéger la sortie"]
```
