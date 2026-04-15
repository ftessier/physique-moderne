# Sujet 3 — Quantification de la lumière

> **Objectif :** Consolider la compréhension du photon comme particule —
> énergie, impulsion, et interactions avec la matière.
> Les exercices sont ordonnés pour **bâtir la confiance** : chaque question commence
> par une porte d'entrée accessible avant de monter en difficulté.

## Exercice 1 — Le détective quantique (effet photoélectrique)

Dans un laboratoire, on éclaire une surface métallique inconnue avec de la lumière monochromatique et on mesure l'énergie cinétique maximale $E_k$ des électrons éjectés pour différentes fréquences $f$ :

| $f$ ($\times 10^{14}$ Hz) | $E_k^{\max}$ (eV) |
| ------------------------- | ----------------- |
| $6.0$                     | $0.21$            |
| $8.0$                     | $1.04$            |
| $10.0$                    | $1.86$            |
| $12.0$                    | $2.69$            |

Données : $h = 6.626 \times 10^{-34}$ J·s $= 4.136 \times 10^{-15}$ eV·s, $\;1 \text{ eV} = 1.602 \times 10^{-19}$ J.

**(a)** La relation $E_k^{\max} = hf - \phi$ est une droite en $f$. Sans calcul détaillé, en regardant le tableau : quand $f$ augmente de $2.0 \times 10^{14}$ Hz, de combien augmente $E_k^{\max}$ ? Est-ce constant ? Qu'est-ce que cela confirme ?

**(b)** Déterminez le travail d'extraction $\phi$ du métal, en eV.

**(c)** En déduire la fréquence seuil $f_0$ et la longueur d'onde seuil $\lambda_0$.

**(d)** On remplace la lumière par un laser très intense ($10^{18}$ photons/s) de fréquence $f = 4.0 \times 10^{14}$ Hz. Observe-t-on un effet photoélectrique ? Justifiez en une phrase — c'est la phrase qui compte, pas le calcul.

<details>
<summary><strong>Solution</strong></summary>

**(a)** Les augmentations de $E_k^{\max}$ :

- De $6.0$ à $8.0$ : $\Delta E_k = 1.04 - 0.21 = 0.83$ eV
- De $8.0$ à $10.0$ : $\Delta E_k = 1.86 - 1.04 = 0.82$ eV
- De $10.0$ à $12.0$ : $\Delta E_k = 2.69 - 1.86 = 0.83$ eV

C'est essentiellement **constant** ($\approx 0.83$ eV par $2.0 \times 10^{14}$ Hz). Cela confirme la relation **linéaire** $E_k = hf - \phi$ : la pente est $h$, et elle est universelle.

Bonus : $h \approx \frac{0.83 \text{ eV}}{2.0 \times 10^{14} \text{ Hz}} \approx 4.15 \times 10^{-15}$ eV·s, en excellent accord avec la valeur connue. ✓

**(b)** En utilisant n'importe quel point, par exemple $(f, E_k) = (6.0 \times 10^{14},\; 0.21)$ :

$$\phi = hf - E_k^{\max} = (4.136 \times 10^{-15})(6.0 \times 10^{14}) - 0.21 = 2.48 - 0.21 = 2.27 \text{ eV}$$

Vérification avec un autre point : $(10.0 \times 10^{14},\; 1.86)$ :

$$\phi = 4.136 - 1.86 = 2.28 \text{ eV} \quad \checkmark$$

Donc $\phi \approx 2.27$ eV (cohérent avec le potassium ou le sodium).

**(c)**

$$f_0 = \frac{\phi}{h} = \frac{2.27}{4.136 \times 10^{-15}} \approx 5.49 \times 10^{14} \text{ Hz}$$

$$\lambda_0 = \frac{c}{f_0} = \frac{3.0 \times 10^8}{5.49 \times 10^{14}} \approx 546 \text{ nm}$$

C'est dans le vert — la lumière visible peut provoquer l'effet photoélectrique sur ce métal.

**(d)** **Non.** La fréquence $f = 4.0 \times 10^{14}$ Hz est **inférieure** à la fréquence seuil $f_0 \approx 5.49 \times 10^{14}$ Hz. Aucun électron n'est éjecté, quelle que soit l'intensité. C'est précisément le résultat qu'une théorie ondulatoire classique ne peut pas expliquer : l'intensité apporte plus de photons, mais chaque photon n'a pas assez d'énergie individuellement pour arracher un électron.

> **Ce qu'on retient :** Si tu as réussi (a) en repérant la linéarité dans le tableau, tu as déjà l'intuition physique. Le reste n'est que de l'arithmétique soignée !

</details>

## Exercice 2 — Le photon recule (diffusion Compton)

Un photon X d'énergie $E_0 = 80.0$ keV frappe un électron libre au repos et est diffusé à un angle $\theta = 90°$ par rapport à sa direction incidente.

Données : $m_e c^2 = 511$ keV, $\;h = 6.626 \times 10^{-34}$ J·s, $\;c = 3.0 \times 10^8$ m/s.

Formule de Compton : $\Delta\lambda = \dfrac{h}{m_e c}(1 - \cos\theta)$

**(a)** Commençons par l'intuition. Avant tout calcul : le photon diffusé aura-t-il une longueur d'onde plus grande ou plus petite que le photon incident ? Justifiez en termes d'énergie (une phrase suffit).

**(b)** Calculez la longueur d'onde du photon incident $\lambda_0$ et celle du photon diffusé $\lambda'$.

**(c)** Quelle est l'énergie du photon diffusé $E'$ ? Quel pourcentage de l'énergie initiale le photon a-t-il perdu ?

**(d)** En déduire l'énergie cinétique de l'électron de recul.

**(e)** Reprenons la même situation mais avec un photon visible ($E_0 = 2.0$ eV). Calculez la variation relative $\Delta\lambda / \lambda_0$. Pourquoi la diffusion Compton est-elle inobservable avec de la lumière visible ?

<details>
<summary><strong>Solution</strong></summary>

**(a)** Le photon cède de l'énergie à l'électron. Son énergie diminue, donc sa fréquence diminue, donc sa **longueur d'onde augmente**. ($\lambda' > \lambda_0$.)

> Bravo si tu as répondu ça sans calcul — c'est le réflexe que l'examen teste.

**(b)** Longueur d'onde incidente :

$$\lambda_0 = \frac{hc}{E_0} = \frac{(4.136 \times 10^{-15})(3.0 \times 10^8)}{80.0 \times 10^3} = \frac{1.241 \times 10^{-6}}{80.0 \times 10^3} \approx 1.551 \times 10^{-11} \text{ m}$$

Ou plus simplement avec $hc \approx 1241$ eV·nm $= 1.241 \times 10^{-9}$ eV·m :

$$\lambda_0 = \frac{1241 \text{ eV·nm}}{80\,000 \text{ eV}} = 0.01551 \text{ nm} = 15.51 \text{ pm}$$

Décalage Compton à $\theta = 90°$ ($\cos 90° = 0$) :

$$\Delta\lambda = \frac{h}{m_e c}(1 - 0) = \frac{h}{m_e c} = 2.426 \text{ pm}$$

(C'est la **longueur d'onde de Compton** de l'électron.)

$$\lambda' = \lambda_0 + \Delta\lambda = 15.51 + 2.43 = 17.94 \text{ pm}$$

**(c)**

$$E' = \frac{hc}{\lambda'} = \frac{1241 \text{ eV·nm}}{0.01794 \text{ nm}} = 69.2 \text{ keV}$$

Perte relative :

$$\frac{E_0 - E'}{E_0} = \frac{80.0 - 69.2}{80.0} \approx 13.5\%$$

Le photon perd environ **14%** de son énergie à $90°$ — un effet très mesurable.

**(d)** Conservation de l'énergie :

$$E_k^{e} = E_0 - E' = 80.0 - 69.2 = 10.8 \text{ keV}$$

**(e)** Pour un photon visible ($E_0 = 2.0$ eV) :

$$\lambda_0 = \frac{1241}{2.0} = 620.5 \text{ nm} = 620\,500 \text{ pm}$$

$$\frac{\Delta\lambda}{\lambda_0} = \frac{2.43}{620\,500} \approx 3.9 \times 10^{-6}$$

Le décalage est de **4 millionièmes** de la longueur d'onde — totalement noyé dans la largeur naturelle des raies spectrales. L'effet Compton n'est mesurable que lorsque $\Delta\lambda$ est une fraction appréciable de $\lambda_0$, ce qui exige $\lambda_0 \sim h/m_e c$, c'est-à-dire des **rayons X ou gamma**.

> **Ce qu'on retient :** $\Delta\lambda$ est toujours le même ($\leq 2h/m_ec$) — c'est $\lambda_0$ qui change. Toute la physique est dans le **rapport** $\Delta\lambda / \lambda_0$.

</details>

## Exercice 3 — Photon contre électron : qui porte le plus d'impulsion ?

Cet exercice ne demande qu'une poignée de calculs, mais chacun révèle quelque chose de surprenant.

**(a)** Un photon a une énergie de $2.0$ eV (lumière visible). Calculez son impulsion $p_\gamma$ en kg·m/s.

**(b)** Un électron a également une énergie cinétique de $2.0$ eV. Calculez son impulsion $p_e$ en kg·m/s. (L'approximation non relativiste est-elle valide ici ? Vérifiez.)

**(c)** Calculez le rapport $p_e / p_\gamma$. L'un de ces deux rapports est-il surprenant ? Lequel transporte le plus d'impulsion ?

**(d)** Calculez maintenant la longueur d'onde de de Broglie de l'électron : $\lambda_e = h / p_e$. Comparez à la longueur d'onde du photon $\lambda_\gamma$.

**(e)** Un expérimentateur veut sonder la structure d'un cristal dont l'espacement interatomique est $d \approx 0.2$ nm. Pour observer de la diffraction, il faut $\lambda \lesssim d$. Quelle énergie cinétique minimale faut-il donner à un électron pour y arriver ? Et pour un photon ?

<details>
<summary><strong>Solution</strong></summary>

**(a)** Pour un photon, $E = pc$ :

$$p_\gamma = \frac{E}{c} = \frac{2.0 \times 1.602 \times 10^{-19}}{3.0 \times 10^8} = 1.07 \times 10^{-27} \text{ kg·m/s}$$

**(b)** Vérifions d'abord : $E_k = 2.0$ eV et $m_e c^2 = 511\,000$ eV, donc $E_k / m_e c^2 \approx 4 \times 10^{-6} \ll 1$. Le traitement non relativiste est parfaitement justifié.

$$p_e = \sqrt{2m_e E_k} = \sqrt{2 \times 9.109 \times 10^{-31} \times 3.204 \times 10^{-19}} = \sqrt{5.834 \times 10^{-49}} = 7.64 \times 10^{-25} \text{ kg·m/s}$$

**(c)**

$$\frac{p_e}{p_\gamma} = \frac{7.64 \times 10^{-25}}{1.07 \times 10^{-27}} \approx 714$$

À énergie égale, l'électron transporte environ **700 fois plus d'impulsion** que le photon. C'est parce que le photon voyage à $c$ — il lui faut très peu d'impulsion pour transporter une énergie donnée. L'électron, beaucoup plus lent, doit compenser par une impulsion élevée.

> Résultat contre-intuitif, non ? La plupart des étudiants s'attendent à l'inverse. Mais c'est la relation $E = pc$ vs $E_k = p^2/2m$ qui fait toute la différence.

**(d)**

$$\lambda_e = \frac{h}{p_e} = \frac{6.626 \times 10^{-34}}{7.64 \times 10^{-25}} = 8.67 \times 10^{-10} \text{ m} \approx 0.87 \text{ nm}$$

$$\lambda_\gamma = \frac{hc}{E} = \frac{1241 \text{ eV·nm}}{2.0 \text{ eV}} = 620 \text{ nm}$$

L'électron de $2$ eV a une longueur d'onde **700 fois plus petite** que le photon de même énergie — exactement le même facteur que le rapport d'impulsion (logique : $\lambda = h/p$).

**(e)** Condition : $\lambda \leq 0.2$ nm.

**Pour l'électron :**

$$p_e \geq \frac{h}{\lambda} = \frac{6.626 \times 10^{-34}}{2.0 \times 10^{-10}} = 3.31 \times 10^{-24} \text{ kg·m/s}$$

$$E_k = \frac{p_e^2}{2m_e} = \frac{(3.31 \times 10^{-24})^2}{2 \times 9.109 \times 10^{-31}} = 6.02 \times 10^{-18} \text{ J} \approx 37.6 \text{ eV}$$

**Pour le photon :**

$$E_\gamma = \frac{hc}{\lambda} = \frac{1241 \text{ eV·nm}}{0.2 \text{ nm}} = 6\,205 \text{ eV} \approx 6.2 \text{ keV}$$

Pour sonder la même structure, le photon nécessite environ **165 fois plus d'énergie** que l'électron. C'est pourquoi la diffraction électronique et la microscopie électronique sont si puissantes : les électrons offrent une résolution spatiale élevée à basse énergie.

> **Ce qu'on retient :** Ce résultat est au cœur de la physique moderne — c'est la raison pour laquelle Davisson et Germer ont pu observer la diffraction d'électrons, et pourquoi les microscopes électroniques existent.

</details>


## Exercice 4 — Gymnastique algébrique : dérivation de la formule de Compton (sans valeurs numériques)

> C'est la « boss battle » de ce sujet. La dérivation complète de la formule de Compton
> à partir des lois de conservation est un classique d'examen — et un terrain miné
> d'erreurs algébriques. Chaque étape est détaillée pour identifier les pièges.

Un photon d'énergie $E_0$ et d'impulsion $p_0 = E_0/c$ frappe un électron libre de masse $m$, au repos. Après la collision, le photon est diffusé à un angle $\theta$ avec une énergie $E'$ et une impulsion $p' = E'/c$, et l'électron recule avec une impulsion $\vec{p}_e$.

On veut montrer :

$$\frac{1}{E'} - \frac{1}{E_0} = \frac{1}{mc^2}(1 - \cos\theta)$$

ce qui est équivalent à $\Delta\lambda = \dfrac{h}{mc}(1 - \cos\theta)$.


### Partie A — Mise en place des équations

**(a)** Écrivez la conservation de l'énergie. Attention : l'énergie totale de l'électron après la collision n'est pas $E_k^e$ mais $\sqrt{(p_e c)^2 + (mc^2)^2}$.

**(b)** Écrivez la conservation de l'impulsion selon $x$ (direction incidente) et selon $y$.

<details>
<summary><strong>Solution partie A</strong></summary>

**(a)** Conservation de l'énergie :

$$E_0 + mc^2 = E' + \sqrt{(p_e c)^2 + (mc^2)^2} \quad (1)$$

Le terme $mc^2$ à gauche est l'énergie **totale** de l'électron au repos.

> **Piège courant :** Écrire $E_0 = E' + E_k^e$ (en oubliant l'énergie de masse de l'électron). Cette formule n'est pas fausse en soi ($E_k^e = E_0 - E'$ est correct), mais elle ne permet pas d'éliminer $p_e$ dans les étapes suivantes, parce qu'on a besoin de la relation énergie-impulsion *complète* pour l'électron.

**(b)** Selon $x$ :

$$\frac{E_0}{c} = \frac{E'}{c}\cos\theta + p_e\cos\phi \quad (2)$$

Selon $y$ :

$$0 = \frac{E'}{c}\sin\theta - p_e\sin\phi \quad (3)$$

où $\phi$ est l'angle de recul de l'électron.

</details>


### Partie B — Élimination de l'électron

L'astuce centrale est d'**éliminer** $p_e$ et $\phi$ (qu'on ne veut pas calculer). C'est ici que ça se joue.

**(c)** Isolez $p_e\cos\phi$ de l'équation (2) et $p_e\sin\phi$ de l'équation (3). Élevez les deux au carré et additionnez-les pour obtenir $(p_e c)^2$ en fonction de $E_0$, $E'$ et $\theta$.

<details>
<summary><strong>Indice</strong></summary>

Utilisez $\cos^2\phi + \sin^2\phi = 1$. C'est l'identité qui élimine $\phi$ d'un coup.

</details>

<details>
<summary><strong>Solution partie B</strong></summary>

De (2) : $p_e c\cos\phi = E_0 - E'\cos\theta$

De (3) : $p_e c\sin\phi = E'\sin\theta$

Au carré et addition :

$$(p_e c)^2(\cos^2\phi + \sin^2\phi) = (E_0 - E'\cos\theta)^2 + (E'\sin\theta)^2$$

$$(p_e c)^2 = E_0^2 - 2E_0 E'\cos\theta + E'^2\cos^2\theta + E'^2\sin^2\theta$$

$$(p_e c)^2 = E_0^2 - 2E_0 E'\cos\theta + E'^2 \quad (4)$$

> **Piège courant :** Oublier de développer $(E_0 - E'\cos\theta)^2$ correctement — le double produit $2E_0 E'\cos\theta$ est souvent perdu, ce qui sabote toute la suite. Autre erreur : ne pas reconnaître que $\cos^2\theta + \sin^2\theta = 1$ simplifie les termes en $E'^2$.

</details>


### Partie C — Élimination de $p_e$ via l'énergie

**(d)** Isolez le radical dans l'équation (1) et élevez au carré pour obtenir une deuxième expression de $(p_e c)^2$.

<details>
<summary><strong>Solution partie C</strong></summary>

De (1) :

$$\sqrt{(p_e c)^2 + (mc^2)^2} = E_0 - E' + mc^2$$

Au carré :

$$(p_e c)^2 + (mc^2)^2 = (E_0 - E' + mc^2)^2$$

$$(p_e c)^2 = (E_0 - E')^2 + 2(E_0 - E')\,mc^2 + \cancel{(mc^2)^2} - \cancel{(mc^2)^2}$$

$$(p_e c)^2 = (E_0 - E')^2 + 2(E_0 - E')\,mc^2 \quad (5)$$

> **Piège courant :** Le développement de $(E_0 - E' + mc^2)^2$ a **trois** termes croisés, pas deux. L'erreur la plus commune est d'écrire $(E_0 - E')^2 + (mc^2)^2$ en oubliant $2(E_0 - E')mc^2$ — exactement le même piège que dans l'exercice 4 du sujet 2, partie C. C'est la même structure algébrique : $(a + b)^2 = a^2 + 2ab + b^2$.

</details>


### Partie D — Le coup de grâce

**(e)** Égalisez les expressions (4) et (5). Développez $(E_0 - E')^2$ dans (5), simplifiez, et montrez que tout se réduit à :

$$\frac{1}{E'} - \frac{1}{E_0} = \frac{1}{mc^2}(1 - \cos\theta)$$

**(f)** En utilisant $E = hc/\lambda$, montrez que cette relation est équivalente à :

$$\lambda' - \lambda_0 = \frac{h}{mc}(1 - \cos\theta)$$

<details>
<summary><strong>Solution partie D</strong></summary>

**(e)** Égalisons (4) et (5) :

$$E_0^2 - 2E_0 E'\cos\theta + E'^2 = (E_0 - E')^2 + 2(E_0 - E')\,mc^2$$

Développons $(E_0 - E')^2 = E_0^2 - 2E_0 E' + E'^2$ à droite :

$$\cancel{E_0^2} - 2E_0 E'\cos\theta + \cancel{E'^2} = \cancel{E_0^2} - 2E_0 E' + \cancel{E'^2} + 2(E_0 - E')\,mc^2$$

$$-2E_0 E'\cos\theta = -2E_0 E' + 2(E_0 - E')\,mc^2$$

Réarrangeons :

$$2E_0 E' - 2E_0 E'\cos\theta = 2(E_0 - E')\,mc^2$$

$$2E_0 E'(1 - \cos\theta) = 2mc^2(E_0 - E')$$

Division par $2E_0 E' mc^2$ :

$$\frac{1 - \cos\theta}{mc^2} = \frac{E_0 - E'}{E_0 E'} = \frac{1}{E'} - \frac{1}{E_0}$$

$$\boxed{\frac{1}{E'} - \frac{1}{E_0} = \frac{1}{mc^2}(1 - \cos\theta)}$$

> **Piège courant :** L'étape où $E_0^2$ et $E'^2$ s'annulent des deux côtés est celle que les étudiants ratent le plus souvent — ils ne développent pas $(E_0 - E')^2$ et restent avec des carrés irréductibles. L'autre piège est de perdre un facteur 2 dans la division finale. **Conseil :** si tu arrives à une expression avec des carrés d'énergie qui ne s'annulent pas, c'est le signe que tu as fait une erreur en amont.

**(f)** On remplace $E_0 = hc/\lambda_0$ et $E' = hc/\lambda'$ :

$$\frac{1}{hc/\lambda'} - \frac{1}{hc/\lambda_0} = \frac{1}{mc^2}(1 - \cos\theta)$$

$$\frac{\lambda'}{hc} - \frac{\lambda_0}{hc} = \frac{1}{mc^2}(1 - \cos\theta)$$

$$\frac{\lambda' - \lambda_0}{hc} = \frac{1}{mc^2}(1 - \cos\theta)$$

$$\boxed{\lambda' - \lambda_0 = \frac{h}{mc}(1 - \cos\theta)}$$

La quantité $\dfrac{h}{mc} = \lambda_C \approx 2.426$ pm est la **longueur d'onde de Compton** de l'électron.

> **Ce qu'on retient :** Tu viens de dériver l'une des formules les plus importantes de la physique moderne en partant uniquement de la conservation de l'énergie et de l'impulsion relativistes. Les mêmes techniques (isoler, élever au carré, éliminer les variables inconnues) reviennent dans presque tous les problèmes de collision/désintégration. Si tu maîtrises cette dérivation, tu maîtrises le *pattern*.

</details>
