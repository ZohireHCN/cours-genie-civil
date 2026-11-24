# Exercices corrigés de mathématiques

[← Retour au sommaire](README.md)

Exercices types. Calculs vérifiés numériquement.

---

## Exercice 1. Système par le pivot de Gauss

$$\begin{cases} 2x + y - z = 8 \\ -3x - y + 2z = -11 \\ -2x + y + 2z = -3 \end{cases}$$

### Correction

- L2 ← L2 + (3/2) L1 : $\tfrac12 y + \tfrac12 z = 1$.
- L3 ← L3 + L1 : $2y + z = 5$.
- L3 ← L3 − 4 L2 : $-z = 1$, donc **z = −1**.
- Remontée : $\tfrac12 y - \tfrac12 = 1$, donc **y = 3** ; $2x + 3 + 1 = 8$, donc **x = 2**.

Vérification dans L2 : −6 − 3 − 2 = −11 ✔.

---

## Exercice 2. Valeurs propres

$A = \begin{pmatrix} 4 & 1 \\ 2 & 3 \end{pmatrix}$. Valeurs propres et vecteurs propres.

### Correction

$$\det(A - \lambda I) = (4-\lambda)(3-\lambda) - 2 = \lambda^2 - 7\lambda + 10 = (\lambda - 5)(\lambda - 2)$$

- λ1 = **5** : $(A - 5I)\vec{v} = 0$ donne −x + y = 0, $\vec{v}_1 = (1 ; 1)$.
- λ2 = **2** : 2x + y = 0, $\vec{v}_2 = (1 ; -2)$.

Contrôles : 5 + 2 = 7 = trace ; 5 × 2 = 10 = det. ✔ (A n'étant pas symétrique, les vecteurs propres ne sont pas orthogonaux.)

---

## Exercice 3. Méthode de Newton

Résoudre $x^3 - 2x - 5 = 0$ en partant de x0 = 2.

### Correction

$f'(x) = 3x^2 - 2$ ; $x_{n+1} = x_n - \dfrac{x_n^3 - 2x_n - 5}{3x_n^2 - 2}$.

| n | xn | f(xn) |
| --- | --- | --- |
| 0 | 2 | −1 |
| 1 | 2,1 | 0,061 |
| 2 | 2,094 568 | 0,000 186 |
| 3 | 2,094 551 | ≈ 0 |

Solution : **x ≈ 2,09455**. Le nombre de décimales justes double à chaque itération.

---

## Exercice 4. Intégration numérique

Calculer $\displaystyle\int_0^1 e^{-x^2}dx$ par les trapèzes et par Simpson avec n = 2 (h = 0,5). Valeur exacte : 0,746 824.

### Correction

f(0) = 1 ; f(0,5) = 0,7788 ; f(1) = 0,3679.

- Trapèzes : $\dfrac{0{,}5}{2}(1 + 2\times0{,}7788 + 0{,}3679) = 0{,}7314$ (erreur 2,1 %).
- Simpson : $\dfrac{0{,}5}{3}(1 + 4\times0{,}7788 + 0{,}3679) = 0{,}7472$ (erreur 0,05 %).

Avec seulement 3 points, Simpson est 40 fois plus précis.

---

## Exercice 5. Pluie de projet (Gumbel)

Les pluies journalières maximales annuelles d'une station suivent une loi de Gumbel de paramètres u = 40 mm et a = 12 mm. Pluie de période de retour 50 ans ? Risque qu'elle soit dépassée au moins une fois pendant les 30 ans de vie d'un ouvrage ?

### Correction

$$x_{50} = 40 - 12\ln\left[-\ln(0{,}98)\right] = 40 + 12\times3{,}902 = 86{,}8\ \text{mm}$$

$$R = 1 - 0{,}98^{30} = 1 - 0{,}545 = 45{,}5\ \%$$

Presque une chance sur deux : la « crue de 50 ans » n'est pas un événement rare à l'échelle de la vie d'un ouvrage.

---

## Exercice 6. Méthode d'Euler

Résoudre y′ = −2y, y(0) = 1, avec h = 0,1, jusqu'à x = 0,3. Comparer à la solution exacte $e^{-2x}$.

### Correction

$y_{n+1} = y_n + 0{,}1\times(-2y_n) = 0{,}8\,y_n$.

| x | Euler | Exact | Erreur |
| --- | --- | --- | --- |
| 0 | 1 | 1 | 0 |
| 0,1 | 0,800 | 0,819 | 2,3 % |
| 0,2 | 0,640 | 0,670 | 4,5 % |
| 0,3 | 0,512 | 0,549 | 6,7 % |

L'erreur s'accumule à chaque pas. En divisant h par 2, on la divise environ par 2.

---

## Exercice 7. Déformée d'une console par intégration

Console de longueur L encastrée en x = 0, charge P à l'extrémité. M(x) = −P (L − x). Trouver la flèche en bout avec $EI\,y'' = M(x)$.

### Correction

$$EI\,y' = -P\left(Lx - \frac{x^2}{2}\right) + C_1 \qquad EI\,y = -P\left(\frac{Lx^2}{2} - \frac{x^3}{6}\right) + C_1x + C_2$$

Encastrement : y(0) = 0 et y′(0) = 0, donc C1 = C2 = 0. En x = L :

$$y(L) = -\frac{P}{EI}\left(\frac{L^3}{2} - \frac{L^3}{6}\right) = -\frac{PL^3}{3EI}$$

On retrouve la formule du formulaire de [RDM](../06-rdm/cours.md) (le signe moins indique une flèche vers le bas).
