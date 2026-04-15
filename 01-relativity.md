# Sujet 1 — Relativité restreinte : temps propre, longueur propre, transformations de Lorentz

> **Objectif :** Trouver la porte d'entrée, pas seulement tourner la manivelle.
> Chaque exercice cible un piège conceptuel fréquent en examen.

## Exercice 1 — Le méson et le détecteur

Un méson traverse un détecteur rectiligne de longueur $L = 4.0 \text{ m}$ (mesurée au labo). L'électronique du détecteur enregistre un temps de transit $\Delta t = 20 \text{ ns}$ entre l'entrée et la sortie du méson.

**(a)** Trouvez la vitesse du méson.

**(b)** Combien de temps le transit a-t-il duré selon le méson ?

**(c)** Quelle est la longueur du détecteur selon le méson ?

<details>
<summary><strong>Indice stratégique</strong></summary>

En (b), demandez-vous : **qui est présent aux deux événements ?** C'est cette question qui détermine qui mesure le temps propre. L'erreur fatale est d'écrire $\Delta t' = \gamma \Delta t$ sans vérifier.

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)** Cinématique pure :

$$v = \frac{L}{\Delta t} = \frac{4.0}{20 \times 10^{-9}} = 2.0 \times 10^8 \text{ m/s} = \frac{2}{3}c$$

**(b)** Les événements « entrée » et « sortie » se produisent à des endroits *différents* dans le labo, mais au *même endroit* pour le méson (il est présent aux deux). C'est donc le méson qui mesure le temps propre $\Delta\tau$.

$$\gamma = \frac{1}{\sqrt{1 - (2/3)^2}} = \frac{1}{\sqrt{5/9}} = \frac{3}{\sqrt{5}} \approx 1.342$$

$$\Delta\tau = \frac{\Delta t}{\gamma} = \frac{20}{\frac{3}{\sqrt{5}}} = \frac{20\sqrt{5}}{3} \approx 14.9 \text{ ns}$$

**(c)** Le détecteur est en mouvement par rapport au méson, donc sa longueur est contractée :

$$L' = \frac{L}{\gamma} = \frac{4.0}{\frac{3}{\sqrt{5}}} = \frac{4\sqrt{5}}{3} \approx 2.98 \text{ m}$$

**Vérification :** $L' = v \cdot \Delta\tau = \frac{2}{3}c \cdot \frac{20\sqrt{5}}{3} \text{ ns} \approx 2.98 \text{ m}$ ✓

</details>

## Exercice 2 — Lorentz obligatoire

Deux événements dans le référentiel $S$ :

| Événement | $x$ | $t$ |
|--|--|--|
| 1 | $0$ | $0$ |
| 2 | $3.0 \text{ al}$ | $5.0 \text{ ans}$ |

Un référentiel $S'$ se déplace à $v = 0.6c$ selon $x$ positif par rapport à $S$.

**(a)** Trouvez $\Delta t'$ dans $S'$ en utilisant la transformation de Lorentz complète.

**(b)** Un étudiant pressé applique « $\Delta t' = \gamma \Delta t = 6.25 \text{ ans}$ ». Montrez que c'est faux et expliquez **en une phrase** pourquoi la formule de dilatation ne s'applique pas ici.

<details>
<summary><strong>Indice stratégique</strong></summary>

Quand est-ce que $\Delta t' = \gamma \Delta t$ est valide ? **Uniquement quand $\Delta x = 0$ dans le référentiel de départ.** Vérifiez cette condition avant d'appliquer la formule.

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)** Transformation de Lorentz complète :

$$\gamma = \frac{1}{\sqrt{1 - 0.6^2}} = \frac{1}{\sqrt{0.64}} = 1.25$$

$$\Delta t' = \gamma\!\left(\Delta t - \frac{v \,\Delta x}{c^2}\right) = 1.25\!\left(5.0 - 0.6 \times 3.0\right) = 1.25 \times 3.2 = \mathbf{4.0 \text{ ans}}$$

**(b)** La formule $\Delta t' = \gamma \Delta t$ suppose que les deux événements se produisent **au même endroit** dans $S$ ($\Delta x = 0$), ce qui en ferait un temps propre. Or ici $\Delta x = 3.0 \text{ al} \neq 0$, donc cette formule est inapplicable. Le terme $\frac{v \,\Delta x}{c^2}$ ne peut pas être ignoré.

Résultat erroné : $6.25$ ans. Résultat correct : $4.0$ ans — une différence de **plus de 50 %**.

</details>

## Exercice 3 — Symétrie dérangeante

Un vaisseau (longueur propre $L_0 = 100 \text{ m}$) passe devant une station spatiale (longueur propre $D_0 = 160 \text{ m}$) à $v = 0.80c$, soit $\gamma = 5/3$.

**(a)** L'observateur de la station mesure la longueur du vaisseau. Résultat ?

**(b)** Le pilote du vaisseau mesure la longueur de la station. Résultat ?

**(c)** Le pilote remarque que la station mesure $96$ m et que son vaisseau mesure $100$ m. Il conclut : « Mon vaisseau est plus long que la station. » L'observateur de la station mesure le vaisseau à $60$ m et la station à $160$ m, et conclut l'inverse. **Y a-t-il contradiction ?** Répondez en identifiant ce que « longueur » signifie opérationnellement.

<details>
<summary><strong>Indice stratégique</strong></summary>

Pour mesurer une longueur, il faut repérer les deux extrémités. Quand faut-il les repérer ? Qu'est-ce que « en même temps » signifie pour chaque observateur ?

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)** Le vaisseau est en mouvement par rapport à la station :

$$L_{\text{vaisseau, station}} = \frac{L_0}{\gamma} = \frac{100}{5/3} = 60 \text{ m}$$

**(b)** La station est en mouvement par rapport au vaisseau :

$$L_{\text{station, vaisseau}} = \frac{D_0}{\gamma} = \frac{160}{5/3} = 96 \text{ m}$$

**(c)** **Il n'y a aucune contradiction.** Mesurer une longueur exige de repérer les positions des deux extrémités **simultanément**. Or la simultanéité est relative :

- La station repère les deux bouts du vaisseau « en même temps » selon ses horloges → $60$ m.
- Le pilote repère les deux bouts de la station « en même temps » selon ses horloges → $96$ m.

Ces deux mesures ne correspondent pas aux mêmes paires d'événements dans l'espace-temps. Chacun a raison dans son référentiel. La « contradiction » naît de l'hypothèse implicite (et fausse) que la simultanéité est absolue.

</details>
