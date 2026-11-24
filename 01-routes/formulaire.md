# Formulaire de Routes

[← Retour au sommaire](README.md)

Unités : V en km/h, v en m/s, longueurs en m, angles en grades sauf mention contraire.

## Tracé en plan

| Notion | Formule |
| --- | --- |
| Alignement droit | $L_{min} = 5v$, $L_{max} = 60v$ |
| Rayon minimal | $R = \dfrac{V^2}{127(f_t + d)}$ |
| Surlargeur par voie | $S = \dfrac{L^2}{2R}$, L ≈ 10 m |

## Raccordement circulaire

α = demi-angle au centre = (200 − A) / 2, A = angle au sommet. Avec des gisements : 2α = |G₂ − G₁|.

| Élément | Formule |
| --- | --- |
| Tangente | $T = R\tan\alpha$ |
| Bissectrice | $B = R\left(\dfrac{1}{\cos\alpha} - 1\right)$ |
| Développée | $D = \dfrac{\pi R (2\alpha)}{200}$ |
| Corde | $c = 2R\sin\alpha$ |
| Flèche | $f = R(1 - \cos\alpha)$ |

## Distances de sécurité

| Notion | Formule |
| --- | --- |
| Freinage | $d_f = 0{,}004\,V^2/f$, f ≈ 0,4 |
| Arrêt en alignement | $d_1 = 0{,}004\,V^2/f + 0{,}55\,V$ (V ≤ 100) |
| Arrêt en courbe (R < 5V) | $d_2 = 0{,}005\,V^2/f + 0{,}55\,V$ |
| Espacement | $e = v\theta + l$, θ = 0,75 s, l = 8 m |
| Visibilité de dépassement | 4V (minimale), 6V (normale) |

## Trafic

| Notion | Formule |
| --- | --- |
| Essieux équivalents | $NE = N \times CAM$ |
| Trafic cumulé | $TC = 365\,N\,r\left(d + \dfrac{t\,d(d-1)}{2}\right)$ |
| Capacité d'une voie | $Q = 1000\,V/d$ (véh/h) |

## Clothoïde

| Notion | Formule |
| --- | --- |
| Définition | $R \times L = A^2$ |
| Angle des tangentes | $\tau = L/(2R)$ (rad) |
| Ripage | $\Delta R \approx L^2/(24R)$ |
| Coordonnées de KE | $X \approx L - L^3/(40R^2)$, $Y \approx L^2/(6R)$ |
| Dévers à l'abscisse x | $d(x) = P_m + (P_M - P_m)\,x/L$ |

## Profil en long

| Notion | Formule |
| --- | --- |
| Rayon vertical (confort, cat. 1-2) | $R_v \ge 0{,}315\,V^2$ |
| Rayon vertical (visibilité) | $R_v = \dfrac{d^2}{2(\sqrt{h_1} + \sqrt{h_2})^2}$ |
| Parabole | $y = x^2/(2R_v)$ |

## Chaussée et terrassements

| Notion | Formule |
| --- | --- |
| Épaisseur CBR | $e = \dfrac{100 + \sqrt{P}(75 + 50\log(N/10))}{I + 5}$ (cm) |
| Épaisseur équivalente | $e = \sum a_i e_i$ |
| Module du sol | $E \approx 5 \times CBR$ (MPa) |
| Cubature | $V = \dfrac{S_1 + S_2}{2}\,d$ |
