# Vidéo de cours d'hydrologie (script et prompts Kling)

[← Retour au sommaire](README.md)

Vidéo d'environ 6 minutes, en 8 scènes. Chaque scène donne la narration (voix off) et un prompt à coller dans Kling (en anglais, Kling comprend mieux). Les clips Kling durent 5 ou 10 s : on les enchaîne au montage (CapCut, DaVinci Resolve) et on ajoute la voix off et les formules en surimpression.

```mermaid
flowchart LR
    S1["1. Le cycle<br/>de l'eau"] --> S2["2. Le bilan<br/>hydrologique"] --> S3["3. Le bassin<br/>versant"] --> S4["4. Forme<br/>et relief"]
    S4 --> S5["5. La pluie<br/>et la période de retour"] --> S6["6. Temps de<br/>concentration"] --> S7["7. Méthode<br/>rationnelle"] --> S8["8. Application<br/>au dalot"]
```

## Conseils de production

- Format 16:9, style « documentaire réaliste » ou « animation 3D pédagogique », le même pour toutes les scènes.
- Les formules ne doivent pas être demandées à Kling (le texte généré est souvent illisible). Ajoutez-les au montage.
- Voix off : enregistrée soi-même ou par synthèse vocale, environ 130 mots par minute.

---

## Scène 1. Le cycle de l'eau (0:00 – 0:45)

**Narration** : « L'eau de la Terre circule sans cesse. Le soleil évapore l'eau des mers, la vapeur forme des nuages, la pluie tombe sur les terres. Une partie s'infiltre, une partie s'évapore à nouveau, et une partie ruisselle vers les oueds. C'est ce ruissellement qui intéresse l'ingénieur. »

**Prompt Kling** :
> Cinematic aerial shot over the Mediterranean coast of southern Tunisia, sun heating the sea, visible water vapor rising, clouds forming over arid mountains, rain falling on hills, water flowing into a dry riverbed (wadi), realistic documentary style, golden hour light, slow camera movement

**Surimpression** : Précipitations → Infiltration / Évaporation / Ruissellement.

## Scène 2. Le bilan hydrologique (0:45 – 1:20)

**Narration** : « Sur un bassin, ce qui entre est égal à ce qui sort plus ce qui est stocké : P égale R plus E plus delta S. Sur une année, le stock varie peu, donc la pluie se partage entre l'écoulement et l'évaporation. »

**Prompt Kling** :
> 3D educational animation of a transparent landscape block showing rain entering from above, water evaporating upward, water flowing out through a river at the bottom, and groundwater stored inside the soil layers, clean white background, soft lighting

**Surimpression** : P = R + E + ΔS.

## Scène 3. Le bassin versant (1:20 – 2:05)

**Narration** : « Le bassin versant est la surface dont toutes les eaux convergent vers un même point, l'exutoire. On le délimite sur une carte topographique en suivant les crêtes : c'est la ligne de partage des eaux. »

**Prompt Kling** :
> Top-down drone view of a mountainous watershed, a glowing blue line tracing the ridge lines around the basin, small streams converging into one main river, camera descends toward the outlet point where a small concrete culvert sits under a road, realistic terrain

**Surimpression** : Surface A (km²), Périmètre P (km), Exutoire.

## Scène 4. Forme et relief (2:05 – 2:50)

**Narration** : « Un bassin ramassé concentre vite ses eaux, un bassin allongé les étale dans le temps. On mesure la forme avec le coefficient de Gravelius, et le relief avec la courbe hypsométrique et l'indice de pente. Plus la pente est forte, plus la crue arrive vite. »

**Prompt Kling** :
> Side-by-side 3D animation of two watersheds, one round and compact, one long and narrow, identical rain falls on both, water reaches the outlet much faster in the round basin, color-coded flow arrows, educational style, white background

**Surimpression** : Kg = 0,28 P / √A. Kg ≈ 1 : rond ; Kg > 1,5 : allongé.

## Scène 5. La pluie et la période de retour (2:50 – 3:40)

**Narration** : « Une pluie de période de retour 50 ans a une chance sur 50 d'être dépassée chaque année. Cela ne veut pas dire qu'elle arrive une fois tous les 50 ans : sur 20 ans, le risque est d'un tiers. Les courbes intensité-durée-fréquence donnent l'intensité de la pluie selon sa durée : plus la pluie est courte, plus elle est intense. »

**Prompt Kling** :
> Heavy short thunderstorm over a small Tunisian town, intense rain on dry ground, then a time-lapse transition to a long gentle rain over the same town, dramatic sky, realistic, 4k

**Surimpression** : P(dépassement) = 1/T ; i = a·t^b (Montana).

## Scène 6. Le temps de concentration (3:40 – 4:25)

**Narration** : « Le temps de concentration est le temps que met la goutte tombée au point le plus éloigné pour atteindre l'exutoire. Si la pluie dure tc, tout le bassin contribue en même temps : c'est elle qui donne le débit maximal. On le calcule par Kirpich, Giandotti ou d'autres formules. »

**Prompt Kling** :
> Animated single blue water droplet falling on the farthest ridge of a 3D watershed model, then traveling down slopes and streams to the outlet, a clock in the corner counting time, other droplets joining along the way, educational animation, clean style

**Surimpression** : Kirpich : tc = 0,0195 L^0,77 I^−0,385 ; Giandotti : tc = (4√A + 1,5L) / (0,8√(Hmoy − Hmin)).

## Scène 7. La méthode rationnelle (4:25 – 5:15)

**Narration** : « Pour un petit bassin, le débit de pointe vaut C fois i fois A divisé par 3,6. C est le coefficient de ruissellement : la part de pluie qui ruisselle. Il est fort sur le bitume et la roche, faible sur les sols cultivés. Si le bassin est mixte, on fait une moyenne pondérée par les surfaces. »

**Prompt Kling** :
> Split-screen comparison of rain falling on an asphalt road where water runs off immediately, and on a plowed olive field where water soaks into the soil, realistic close-up, slow motion raindrops

**Surimpression** : Q = C·i·A / 3,6 (Q en m³/s, i en mm/h, A en km²).

## Scène 8. Application au dalot (5:15 – 6:00)

**Narration** : « Exemple : un bassin de 12,5 kilomètres carrés, C égal 0,52, tc de 156 minutes. L'intensité de 50 ans vaut 16,5 millimètres par heure, et le débit de projet environ 30 mètres cubes par seconde. C'est ce débit que le dalot sous la route doit laisser passer. Avec un autre tc, on trouverait 70 : l'ingénieur doit toujours comparer les méthodes. »

**Prompt Kling** :
> Flash flood in a Tunisian wadi rushing through a concrete box culvert under a rural road, water flows safely through the openings, the road stays dry, an engineer in a safety vest watches from the roadside, realistic cinematic shot

**Surimpression** : Q₅₀ ≈ 30 m³/s → dimensionnement du dalot. Voir [l'examen corrigé](exercices-corriges.md).
