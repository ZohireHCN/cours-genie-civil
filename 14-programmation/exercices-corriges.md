# Exercices corrigés de programmation

[← Retour au sommaire](README.md)

Chaque programme a été exécuté ; la sortie affichée est la sortie réelle. Les exercices reprennent les calculs des autres matières pour vérifier les résultats à la main.

---

## Exercice 1. Débit de projet (hydrologie)

Écrire une fonction `montana(a, b, t)` et une fonction `debit_rationnel(C, i, A)`, puis recalculer le débit de l'[examen d'hydrologie](../02-hydrologie/exercices-corriges.md) (a = 1145, b = −0,84, tc = 156 min, C = 0,52, A = 12,5 km²).

### Correction

```python
import math

def debit_rationnel(C, i, A):
    """Q (m3/s) avec i en mm/h et A en km2."""
    return C * i * A / 3.6

def montana(a, b, t):
    return a * t ** b

i = montana(1145, -0.84, 156)
print(f"i = {i:.1f} mm/h, Q = {debit_rationnel(0.52, i, 12.5):.1f} m3/s")
```

Sortie :

```text
i = 16.5 mm/h, Q = 29.7 m3/s
```

---

## Exercice 2. Gisement et distance (topographie)

Écrire `gisement(xa, ya, xb, yb)` qui renvoie le gisement en grades (entre 0 et 400) et la distance. Tester avec l'exercice 1 de [topographie](../09-topographie/exercices-corriges.md).

### Correction

`math.atan2(dx, dy)` gère automatiquement les quadrants (c'est tout l'intérêt par rapport à `atan(dx / dy)`).

```python
def gisement(xa, ya, xb, yb):
    """Gisement de AB en grades (0 à 400) et distance."""
    dx, dy = xb - xa, yb - ya
    g = math.atan2(dx, dy) * 200 / math.pi
    if g < 0:
        g += 400
    return g, math.hypot(dx, dy)

g, d = gisement(1000, 2000, 1250, 1800)
print(f"G = {g:.4f} gr, D = {d:.2f} m")
```

Sortie :

```text
G = 142.9553 gr, D = 320.16 m
```

---

## Exercice 3. Méthode de Newton

Programmer Newton avec un critère d'arrêt, et résoudre x³ − 2x − 5 = 0.

### Correction

```python
def newton(f, df, x0, tol=1e-8, nmax=50):
    x = x0
    for n in range(nmax):
        dx = f(x) / df(x)
        x = x - dx
        if abs(dx) < tol:
            return x, n + 1
    raise ValueError("pas de convergence")

x, n = newton(lambda x: x**3 - 2*x - 5, lambda x: 3*x**2 - 2, 2)
print(f"x = {x:.6f} en {n} itérations")
```

Sortie :

```text
x = 2.094551 en 4 itérations
```

`lambda` crée une petite fonction anonyme ; on passe des fonctions en paramètre comme n'importe quelle valeur.

---

## Exercice 4. Méthode de Simpson

Programmer Simpson pour n pair et calculer l'intégrale de e^(−x²) entre 0 et 1 avec n = 2 puis n = 10.

### Correction

```python
def simpson(f, a, b, n):
    if n % 2:
        raise ValueError("n doit être pair")
    h = (b - a) / n
    s = f(a) + f(b)
    for k in range(1, n):
        s += (4 if k % 2 else 2) * f(a + k * h)
    return s * h / 3

f = lambda x: math.exp(-x * x)
print(f"{simpson(f, 0, 1, 2):.4f}", f"{simpson(f, 0, 1, 10):.6f}")
```

Sortie :

```text
0.7472 0.746825
```

Avec n = 10, on a 6 décimales justes (valeur exacte 0,746824).

---

## Exercice 5. Statistiques et loi de Gumbel (hydrologie)

Pluies maximales journalières de 10 années (mm) : 52, 38, 61, 45, 70, 33, 48, 57, 41, 66. Calculer moyenne et écart-type, ajuster Gumbel par les moments (a = 0,78 s, u = x̄ − 0,577 a), puis la pluie de 50 ans.

### Correction

```python
def moyenne_ecart_type(valeurs):
    n = len(valeurs)
    m = sum(valeurs) / n
    s = math.sqrt(sum((v - m) ** 2 for v in valeurs) / (n - 1))
    return m, s

pluies = [52, 38, 61, 45, 70, 33, 48, 57, 41, 66]
m, s = moyenne_ecart_type(pluies)
a = 0.78 * s
u = m - 0.577 * a
x50 = u - a * math.log(-math.log(1 - 1/50))
print(f"moyenne = {m:.1f}, s = {s:.2f}, a = {a:.2f}, u = {u:.2f}, P50 = {x50:.1f} mm")
```

Sortie :

```text
moyenne = 51.1, s = 12.30, a = 9.59, u = 45.57, P50 = 83.0 mm
```

Dix années de mesures sont trop peu pour une estimation fiable à 50 ans : dans la réalité, on utilise 20 à 30 ans au moins.

---

## Exercice 6. Réactions d'une poutre (RDM)

Écrire `reactions(L, charges)` pour une poutre sur deux appuis portant une liste de charges concentrées `(P, a)`. Tester avec les exercices de [RDM](../06-rdm/exercices-corriges.md) et de [mécanique des solides](../04-mecanique-des-solides/exercices-corriges.md).

### Correction

```python
def reactions(L, charges):
    """charges : liste de (P en kN, a en m depuis A)."""
    RB = sum(P * a for P, a in charges) / L
    RA = sum(P for P, a in charges) - RB
    return RA, RB

print(reactions(6, [(12, 2)]), reactions(5, [(20, 2)]))
```

Sortie :

```text
(8.0, 4.0) (12.0, 8.0)
```

On retrouve RA = 8 kN, RB = 4 kN et RA = 12 kN, RB = 8 kN.

---

## Exercice 7. Classe de sol (routes)

Écrire `classe_sol(cbr)` qui renvoie la classe S0 à S4 du cours de [Routes](../01-routes/cours.md), et l'appliquer à une liste de valeurs.

### Correction

```python
def classe_sol(cbr):
    if cbr < 5:
        return "S4"
    elif cbr < 10:
        return "S3"
    elif cbr < 25:
        return "S2"
    elif cbr < 40:
        return "S1"
    else:
        return "S0"

print([classe_sol(c) for c in (3, 8, 15, 30, 50)])
```

Sortie :

```text
['S4', 'S3', 'S2', 'S1', 'S0']
```

L'ordre des tests compte : on part du plus petit seuil, et chaque `elif` n'est évalué que si les précédents sont faux.
