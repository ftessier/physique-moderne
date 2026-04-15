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

## Exercice 4 — Gymnastique algébrique (sans valeurs numériques)

> Cet exercice est long à dessein. Chaque partie cible un piège algébrique courant.
> Tout est symbolique : $v$, $c$, $\gamma$, $\beta = v/c$.

Un référentiel $S'$ se déplace à vitesse $v$ selon l'axe $x$ positif par rapport au référentiel $S$. Deux événements sont observés dans $S$ :

- Événement $A$ : $(x_A,\, t_A)$
- Événement $B$ : $(x_B,\, t_B)$
On pose $\Delta x = x_B - x_A$ et $\Delta t = t_B - t_A$.


### Partie A — Identités utiles de $\gamma$

**(a)** À partir de la définition $\gamma = \dfrac{1}{\sqrt{1 - \beta^2}}$, démontrez les trois identités suivantes :

$$\text{(i)}\ \ \frac{1}{\gamma^2} = 1 - \beta^2 \qquad \text{(ii)}\ \ \gamma^2 \beta^2 = \gamma^2 - 1 \qquad \text{(iii)}\ \ \gamma = \frac{1}{\gamma(1-\beta^2)}$$

<details>
<summary><strong>Solution partie A</strong></summary>

**(i)** Direct :

$$\gamma^2 = \frac{1}{1-\beta^2} \implies \frac{1}{\gamma^2} = 1 - \beta^2$$

**(ii)** On part de (i) :

$$\gamma^2(1 - \beta^2) = 1 \implies \gamma^2 - \gamma^2\beta^2 = 1 \implies \gamma^2\beta^2 = \gamma^2 - 1$$

**(iii)** De (i), $\gamma(1 - \beta^2) = \frac{1}{\gamma}$, donc $\frac{1}{\gamma(1 - \beta^2)} = \gamma$.

> **Piège courant :** L'identité (ii) est celle qu'on oublie le plus souvent, et elle est indispensable pour simplifier des expressions qui contiennent $\gamma^2 \beta^2$. Les étudiants qui ne la connaissent pas se retrouvent bloqués dans les simplifications des parties suivantes.

</details>

### Partie B — Retrouver la dilatation du temps

**(b)** Écrivez la transformation de Lorentz pour $\Delta t'$ en fonction de $\Delta t$, $\Delta x$, $v$ et $c$.

**(c)** Supposons que les deux événements se produisent **au même endroit dans $S'$**, c'est-à-dire $\Delta x' = 0$. Montrez, en partant de la transformation de $\Delta x'$, que cette condition impose $\Delta x = v\,\Delta t$. Substituez dans l'expression de $\Delta t'$ et simplifiez **jusqu'au bout** pour obtenir :

$$\Delta t = \gamma\,\Delta t'$$

c'est-à-dire la formule de dilatation du temps, où $\Delta t'$ est le temps propre.

<details>
<summary><strong>Solution partie B</strong></summary>

**(b)**

$$\Delta t' = \gamma\!\left(\Delta t - \frac{v\,\Delta x}{c^2}\right)$$

**(c)** La transformation de $\Delta x'$ :

$$\Delta x' = \gamma(\Delta x - v\,\Delta t)$$

Si $\Delta x' = 0$ : $\Delta x = v\,\Delta t$.

Substitution dans $\Delta t'$ :

$$\Delta t' = \gamma\!\left(\Delta t - \frac{v \cdot v\,\Delta t}{c^2}\right) = \gamma\,\Delta t\!\left(1 - \frac{v^2}{c^2}\right) = \gamma\,\Delta t\!\left(1 - \beta^2\right)$$

En utilisant l'identité $\gamma(1 - \beta^2) = \frac{1}{\gamma}$ :

$$\Delta t' = \frac{\Delta t}{\gamma}$$

Donc $\Delta t = \gamma\,\Delta t'$, ce qui est bien la dilatation du temps.

> **Piège courant :** L'étape critique est la simplification de $\gamma(1 - \beta^2)$. Un étudiant qui ne voit pas cette simplification reste avec un $\gamma$ en trop et obtient $\gamma^2$ au lieu de $\gamma$ — erreur très fréquente. Autre erreur classique : oublier que c'est $\Delta x' = 0$ (pas $\Delta x = 0$) qui définit le temps propre dans $S'$.

</details>

### Partie C — La transformation inverse

**(d)** On donne les transformations de Lorentz :

$$\Delta x' = \gamma(\Delta x - v\,\Delta t) \qquad \Delta t' = \gamma\!\left(\Delta t - \frac{v\,\Delta x}{c^2}\right)$$

En résolvant ce système pour $\Delta x$ et $\Delta t$ en fonction de $\Delta x'$ et $\Delta t'$, montrez **algébriquement** que la transformation inverse est :

$$\Delta x = \gamma(\Delta x' + v\,\Delta t') \qquad \Delta t = \gamma\!\left(\Delta t' + \frac{v\,\Delta x'}{c^2}\right)$$

c'est-à-dire la même transformation avec $v \to -v$.

<details>
<summary><strong>Indice</strong></summary>

Isolez $\Delta x$ à partir de la première équation, puis substituez dans la deuxième. Vous aurez besoin de l'identité $\gamma^2(1 - \beta^2) = 1$. L'algèbre est un peu lourde — c'est voulu.

</details>
<details>
<summary><strong>Solution partie C</strong></summary>

De la première équation :

$$\Delta x' = \gamma(\Delta x - v\,\Delta t) \implies \Delta x = \frac{\Delta x'}{\gamma} + v\,\Delta t \quad (*)$$

Substitution de $(*)$ dans la deuxième équation :

$$\Delta t' = \gamma\!\left(\Delta t - \frac{v}{c^2}\!\left(\frac{\Delta x'}{\gamma} + v\,\Delta t\right)\right)$$

$$= \gamma\,\Delta t - \frac{v\,\Delta x'}{c^2} - \frac{\gamma v^2}{c^2}\,\Delta t$$

$$= \gamma\,\Delta t\!\left(1 - \frac{v^2}{c^2}\right) - \frac{v\,\Delta x'}{c^2}$$

$$= \gamma\,\Delta t(1-\beta^2) - \frac{v\,\Delta x'}{c^2} = \frac{\Delta t}{\gamma} - \frac{v\,\Delta x'}{c^2}$$

On résout pour $\Delta t$ :

$$\Delta t' + \frac{v\,\Delta x'}{c^2} = \frac{\Delta t}{\gamma} \implies \boxed{\Delta t = \gamma\!\left(\Delta t' + \frac{v\,\Delta x'}{c^2}\right)}$$

En reportant dans $(*)$ :

$$\Delta x = \frac{\Delta x'}{\gamma} + v\gamma\!\left(\Delta t' + \frac{v\,\Delta x'}{c^2}\right) = \frac{\Delta x'}{\gamma} + \gamma v\,\Delta t' + \gamma\frac{v^2}{c^2}\,\Delta x'$$

$$= \Delta x'\!\left(\frac{1}{\gamma} + \gamma\beta^2\right) + \gamma v\,\Delta t'$$

Or $\frac{1}{\gamma} + \gamma\beta^2 = \frac{1 + \gamma^2\beta^2}{\gamma} = \frac{1 + \gamma^2 - 1}{\gamma} = \frac{\gamma^2}{\gamma} = \gamma$

(On a utilisé l'identité $\gamma^2\beta^2 = \gamma^2 - 1$ ici !)

$$\boxed{\Delta x = \gamma(\Delta x' + v\,\Delta t')}$$

> **Piège courant :** L'erreur la plus fréquente est de croire que la transformation inverse s'obtient en « divisant par $\gamma$ ». Ce n'est pas le cas : c'est bien $v \to -v$ avec un $\gamma$ qui **multiplie** toujours. L'étape $\frac{1}{\gamma} + \gamma\beta^2 = \gamma$ est celle où 90% des étudiants se perdent sans l'identité (ii).

</details>

### Partie D — Addition relativiste des vitesses

**(e)** Un objet se déplace à vitesse $u$ dans $S$ (selon $x$ positif). En utilisant $u = \Delta x / \Delta t$ et $u' = \Delta x' / \Delta t'$, et les transformations de Lorentz, dérivez la formule d'addition des vitesses :

$$u' = \frac{u - v}{1 - \dfrac{uv}{c^2}}$$

**(f)** Vérifiez que si $u = c$, alors $u' = c$ quel que soit $v$. Montrez chaque étape algébrique.

**(g)** Prenez la limite non relativiste ($v \ll c$ et $u \ll c$). Quelle formule classique retrouvez-vous ?

<details>
<summary><strong>Solution partie D</strong></summary>

**(e)**

$$u' = \frac{\Delta x'}{\Delta t'} = \frac{\gamma(\Delta x - v\,\Delta t)}{\gamma\!\left(\Delta t - \dfrac{v\,\Delta x}{c^2}\right)}$$

Les $\gamma$ se simplifient :

$$u' = \frac{\Delta x - v\,\Delta t}{\Delta t - \dfrac{v\,\Delta x}{c^2}}$$

On divise numérateur et dénominateur par $\Delta t$ :

$$u' = \frac{\dfrac{\Delta x}{\Delta t} - v}{1 - \dfrac{v}{c^2}\dfrac{\Delta x}{\Delta t}} = \frac{u - v}{1 - \dfrac{uv}{c^2}}$$

> **Piège courant :** Oublier de simplifier les $\gamma$ est l'erreur la plus fréquente — les étudiants traînent des $\gamma^2$ dans toute la suite et n'arrivent jamais à simplifier. L'autre erreur classique est d'écrire $\frac{\Delta x}{\Delta t'}$ au lieu de $\frac{\Delta x'}{\Delta t'}$ pour définir $u'$.

**(f)** Si $u = c$ :

$$u' = \frac{c - v}{1 - \dfrac{cv}{c^2}} = \frac{c - v}{1 - \dfrac{v}{c}} = \frac{c - v}{\dfrac{c - v}{c}} = c$$

La vitesse de la lumière est la même dans tous les référentiels. ✓

> **Piège courant :** Certains étudiants mettent $u = c$ uniquement au numérateur et oublient de le substituer au dénominateur, ou bien simplifient $\frac{c-v}{c-v}$ directement sans passer par la mise au même dénominateur.

**(g)** Si $v \ll c$ et $u \ll c$, alors $\frac{uv}{c^2} \approx 0$ et :

$$u' \approx \frac{u - v}{1} = u - v$$

C'est la **transformation galiléenne des vitesses**, $u' = u - v$. ✓

</details>

### Partie E — L'intervalle invariant

**(h)** Calculez la quantité $c^2\Delta t'^2 - \Delta x'^2$ en substituant les transformations de Lorentz. En développant et simplifiant (c'est le calcul le plus long de cet exercice), montrez que :

$$c^2\Delta t'^2 - \Delta x'^2 = c^2\Delta t^2 - \Delta x^2$$

L'intervalle d'espace-temps est le même dans les deux référentiels.

<details>
<summary><strong>Indice</strong></summary>

Développez les carrés soigneusement. Vous obtiendrez des termes en $\gamma^2 c^2\Delta t^2$, $\gamma^2 \Delta x^2$, $\gamma^2 \frac{v^2}{c^2}\Delta x^2$, $\gamma^2 v^2 \Delta t^2$ et des termes croisés en $\gamma^2 v\,\Delta x\,\Delta t$. Les termes croisés doivent s'annuler. Ensuite, factorisez par $\gamma^2$ et utilisez $\gamma^2(1 - \beta^2) = 1$.

</details>
<details>
<summary><strong>Solution partie E</strong></summary>

$$c^2\Delta t'^2 = c^2\gamma^2\!\left(\Delta t - \frac{v\,\Delta x}{c^2}\right)^2 = \gamma^2\!\left(c^2\Delta t^2 - 2v\,\Delta x\,\Delta t + \frac{v^2\Delta x^2}{c^2}\right)$$

$$\Delta x'^2 = \gamma^2(\Delta x - v\,\Delta t)^2 = \gamma^2\!\left(\Delta x^2 - 2v\,\Delta x\,\Delta t + v^2\Delta t^2\right)$$

Soustraction :

$$c^2\Delta t'^2 - \Delta x'^2 = \gamma^2\!\left(c^2\Delta t^2 \cancel{- 2v\,\Delta x\,\Delta t} + \frac{v^2\Delta x^2}{c^2} - \Delta x^2 \cancel{+ 2v\,\Delta x\,\Delta t} - v^2\Delta t^2\right)$$

Les termes croisés s'annulent. Il reste :

$$= \gamma^2\!\left(c^2\Delta t^2 - v^2\Delta t^2 - \Delta x^2 + \frac{v^2}{c^2}\Delta x^2\right)$$

$$= \gamma^2\!\left(\Delta t^2(c^2 - v^2) - \Delta x^2\!\left(1 - \frac{v^2}{c^2}\right)\right)$$

$$= \gamma^2(1 - \beta^2)\!\left(c^2\Delta t^2 - \Delta x^2\right)$$

Or $\gamma^2(1 - \beta^2) = 1$, donc :

$$\boxed{c^2\Delta t'^2 - \Delta x'^2 = c^2\Delta t^2 - \Delta x^2}$$

> **Piège courant :** L'erreur fatale est un signe dans le développement du carré de $\Delta t'$, où le facteur $c^2$ à l'extérieur de la parenthèse interagit avec le $\frac{v}{c^2}$ à l'intérieur. Beaucoup d'étudiants perdent un facteur $c^2$ à cette étape et ne retrouvent jamais l'annulation. L'autre piège est de ne pas factoriser $(1 - \beta^2)$ simultanément des deux termes — il faut le voir dans $\Delta t^2$ **et** dans $\Delta x^2$ en même temps.

</details>
