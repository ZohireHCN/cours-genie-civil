# Formulaire de mécanique des solides

[← Retour au sommaire](README.md)

## Torseurs

| Notion | Formule |
| --- | --- |
| Transport du moment (Varignon, « BABAR ») | $\vec{M}_B = \vec{M}_A + \vec{BA}\wedge\vec{R}$ |
| Moment d'une force F appliquée en A | $\vec{M}_B(\vec{F}) = \vec{BA}\wedge\vec{F}$ |
| Moment en plan | $M = \pm F\,d$ |
| Comoment | $\{\mathcal{T}_1\}\otimes\{\mathcal{T}_2\} = \vec{R}_1\cdot\vec{M}_{2,A} + \vec{R}_2\cdot\vec{M}_{1,A}$ |

## Statique

| Notion | Formule |
| --- | --- |
| PFS | $\{\mathcal{T}(\bar{E}\to E)\} = \{0\}$ : $\sum\vec{F} = \vec{0}$, $\sum\vec{M}_A = \vec{0}$ |
| Problème plan | 3 équations : $\sum X = 0$, $\sum Y = 0$, $\sum M_z = 0$ |
| Actions mutuelles | $\{\mathcal{T}(1\to2)\} = -\{\mathcal{T}(2\to1)\}$ |
| Coulomb, adhérence | $T \le f\,N$ |
| Coulomb, glissement | $T = f\,N$, $\tan\varphi = f$ |
| Liaison | ddl + inconnues statiques = 6 |

## Cinématique

| Notion | Formule |
| --- | --- |
| Formule de Bour | $\left.\dfrac{d\vec{U}}{dt}\right|_{0} = \left.\dfrac{d\vec{U}}{dt}\right|_{1} + \vec{\Omega}(1/0)\wedge\vec{U}$ |
| Rotation plane | $\vec{\Omega}(1/0) = \dot\theta\,\vec{z}$ |
| Champ des vitesses | $\vec{V}(B) = \vec{V}(A) + \vec{BA}\wedge\vec{\Omega}$ |
| Équiprojectivité | $\vec{V}(A)\cdot\vec{AB} = \vec{V}(B)\cdot\vec{AB}$ |
| Composition | $\vec{V}(M\in2/0) = \vec{V}(M\in2/1) + \vec{V}(M\in1/0)$ ; $\vec{\Omega}(2/0) = \vec{\Omega}(2/1) + \vec{\Omega}(1/0)$ |
| Roulement sans glissement | $\vec{V}(I\in1/0) = \vec{0}$ ; $V_{centre} = R\omega$ |
| Rotation autour d'un axe fixe | $V = r\omega$, $a_n = r\omega^2$, $a_t = r\dot\omega$ |

## Cinétique

| Notion | Formule |
| --- | --- |
| Centre d'inertie | $\vec{OG} = \dfrac{\sum m_i\vec{OG_i}}{\sum m_i}$ |
| Moments d'inertie | $A = \int(y^2+z^2)dm$, $B = \int(x^2+z^2)dm$, $C = \int(x^2+y^2)dm$ |
| Huygens | $J_\Delta = J_{\Delta_G} + m\,d^2$ |
| Torseur cinétique | $\{m\vec{V}_G \; ; \; \vec{\sigma}_A\}$, $\vec{\sigma}_G = I(G)\vec{\Omega}$ |
| Torseur dynamique | $\{m\vec{\Gamma}_G \; ; \; \vec{\delta}_A\}$, $\vec{\delta}_G = d\vec{\sigma}_G/dt$ |
| Énergie cinétique | $T = \tfrac12 mV_G^2 + \tfrac12\vec{\Omega}\cdot I(G)\vec{\Omega}$ |

| Solide | Moment d'inertie |
| --- | --- |
| Tige L, au centre | $mL^2/12$ |
| Tige L, à l'extrémité | $mL^2/3$ |
| Disque plein R | $mR^2/2$ |
| Cerceau R | $mR^2$ |
| Sphère pleine R | $2mR^2/5$ |

## Dynamique

| Notion | Formule |
| --- | --- |
| PFD | $\{\mathcal{D}(E/R_g)\} = \{\mathcal{T}(\bar{E}\to E)\}$ |
| Résultante dynamique | $m\vec{\Gamma}_G = \sum\vec{F}_{ext}$ |
| Rotation autour d'un axe fixe | $J_\Delta\ddot\theta = \sum M_\Delta$ |
| Pendule simple | $\ddot\theta + (g/L)\sin\theta = 0$ ; $T_0 = 2\pi\sqrt{L/g}$ |
| Énergie cinétique | $dT/dt = P_{ext} + P_{int}$ |
