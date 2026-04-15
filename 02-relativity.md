# Sujet 2 — Relativité restreinte : masse-énergie, fission nucléaire, désintégration

> **Objectif :** Savoir naviguer entre énergie de masse, énergie cinétique et énergie totale,
> et appliquer la conservation de l'énergie-impulsion à des processus nucléaires et de désintégration.

## Exercice 1 — Le prix d'un café

On chauffe une tasse de café (masse d'eau $m = 250 \text{ g}$) de $20°\text{C}$ à $80°\text{C}$.

Données : $c_{\text{eau}} = 4.18 \text{ J/(g°C)}$

**(a)** Calculez l'énergie thermique $Q$ fournie à l'eau.

**(b)** De combien la masse de l'eau augmente-t-elle, en kg ?

**(c)** Un noyau d'uranium 235 qui fissionne libère environ $200 \text{ MeV}$. Combien de fissions faudrait-il pour fournir l'énergie $Q$ calculée en (a) ?

**(d)** Quel est le défaut de masse $\Delta m$ correspondant à **une seule** fission de $200 \text{ MeV}$ ? Comparez à la masse d'un proton ($m_p \approx 1.67 \times 10^{-27} \text{ kg}$).

<details>
<summary><strong>Indice stratégique</strong></summary>

En (b), l'énergie ajoutée est de l'énergie interne — elle contribue à la masse du système via $E = mc^2$. Le résultat sera ridiculement petit. C'est précisément le point : comprendre *pourquoi* $E = mc^2$ est imperceptible au quotidien mais dévastateur au nucléaire. En (d), pensez à convertir les MeV en joules d'abord.

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)**

$$Q = mc\,\Delta T = 250 \times 4.18 \times 60 = 62\,700 \text{ J} \approx 62.7 \text{ kJ}$$

**(b)**

$$\Delta m = \frac{Q}{c^2} = \frac{62\,700}{(3.0 \times 10^8)^2} = \frac{62\,700}{9.0 \times 10^{16}} \approx 7.0 \times 10^{-13} \text{ kg}$$

C'est environ $0.7 \text{ pg}$ (picogrammes) — totalement immesurable, ce qui explique pourquoi $E = mc^2$ est invisible en thermodynamique quotidienne.

**(c)**

$$200 \text{ MeV} = 200 \times 1.602 \times 10^{-13} \text{ J} = 3.204 \times 10^{-11} \text{ J}$$

$$N = \frac{Q}{E_{\text{fission}}} = \frac{62\,700}{3.204 \times 10^{-11}} \approx 1.96 \times 10^{15} \text{ fissions}$$

Environ $2 \times 10^{15}$ fissions — un nombre colossal, mais correspondant à une quantité de matière infime (~$0.8 \text{ µg}$ d'U-235).

**(d)**

$$\Delta m = \frac{E_{\text{fission}}}{c^2} = \frac{3.204 \times 10^{-11}}{9.0 \times 10^{16}} \approx 3.56 \times 10^{-28} \text{ kg}$$

$$\frac{\Delta m}{m_p} = \frac{3.56 \times 10^{-28}}{1.67 \times 10^{-27}} \approx 0.21$$

Le défaut de masse d'une fission est environ **un cinquième** de la masse d'un proton — cette fois, $\Delta m$ est une fraction appréciable de la masse des constituants. C'est pourquoi $E = mc^2$ est spectaculaire à l'échelle nucléaire.

</details>

## Exercice 2 — Fission asymétrique

Un noyau d'uranium 235, **au repos**, absorbe un neutron thermique (énergie cinétique négligeable) et fissionne selon :

$${}^{235}_{\ 92}\text{U} + {}^{1}_{0}\text{n} \;\longrightarrow\; {}^{140}_{\ 54}\text{Xe} + {}^{94}_{\ 38}\text{Sr} + 2\,{}^{1}_{0}\text{n}$$

Masses atomiques :

| Particule | Masse (u) |
|-----------|-----------|
| ${}^{235}\text{U}$ | $235.0439$ |
| ${}^{1}\text{n}$ | $1.00866$ |
| ${}^{140}\text{Xe}$ | $139.9216$ |
| ${}^{94}\text{Sr}$ | $93.9154$ |

Donnée : $1 \text{ u} = 931.5 \text{ MeV}/c^2$

**(a)** Vérifiez que le nombre de nucléons et la charge sont conservés.

**(b)** Calculez le défaut de masse $\Delta m$ en unités de masse atomique.

**(c)** En déduire l'énergie libérée $Q$ en MeV.

**(d)** Si toute cette énergie se retrouve sous forme d'énergie cinétique des produits (les deux fragments + les deux neutrons), peut-on traiter le problème de manière non relativiste ? Justifiez en estimant $v/c$ pour le fragment de xénon.

<details>
<summary><strong>Indice stratégique</strong></summary>

Le piège en (b) : n'oubliez pas qu'il y a **deux** neutrons produits et **un** neutron absorbé. Comptez soigneusement les masses initiales et finales. En (d), la question est : est-ce que $E_k \ll m c^2$ pour les fragments ?

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)** Vérification :
- Nucléons : $235 + 1 = 140 + 94 + 2 \times 1$ → $236 = 236$ ✓
- Charge : $92 + 0 = 54 + 38 + 0$ → $92 = 92$ ✓

**(b)**

$$m_{\text{initiale}} = 235.0439 + 1.00866 = 236.05256 \text{ u}$$

$$m_{\text{finale}} = 139.9216 + 93.9154 + 2 \times 1.00866 = 235.85366 \text{ u}$$

$$\Delta m = 236.05256 - 235.85366 = 0.19890 \text{ u}$$

**(c)**

$$Q = \Delta m \times 931.5 = 0.19890 \times 931.5 \approx 185.3 \text{ MeV}$$

**(d)** Estimation pour le xénon : en supposant (approximation grossière) que le Xe emporte environ la moitié de l'énergie cinétique :

$$E_k^{\text{Xe}} \sim \frac{185}{2} \approx 93 \text{ MeV}$$

$$m_{\text{Xe}}\,c^2 = 140 \times 931.5 \approx 130\,400 \text{ MeV}$$

$$\frac{E_k}{mc^2} \approx \frac{93}{130\,400} \approx 7 \times 10^{-4} \ll 1$$

Donc $v/c \approx \sqrt{2 E_k / mc^2} \approx 0.038$ — soit environ $4\%$ de $c$. **Le traitement non relativiste est amplement justifié** pour les fragments lourds. (Pour les neutrons, $E_k/m_n c^2$ est plus grand mais reste $\ll 1$.)

</details>

## Exercice 3 — Désintégration du pion neutre

Un pion neutre ($\pi^0$) **au repos** se désintègre en deux photons :

$$\pi^0 \;\longrightarrow\; \gamma + \gamma$$

Masse du pion : $m_{\pi} = 135.0 \text{ MeV}/c^2$

Rappels : pour un photon, $E = pc$ (masse nulle). La relation énergie-impulsion relativiste est $E^2 = (pc)^2 + (mc^2)^2$.

**(a)** En utilisant la conservation de l'impulsion dans le référentiel de repos du pion, que pouvez-vous déduire sur les directions et les énergies des deux photons ?

**(b)** Un étudiant propose plutôt la désintégration en un **seul** photon : $\pi^0 \to \gamma$. Montrez que c'est impossible en écrivant **séparément** la conservation de l'énergie et la conservation de l'impulsion.

**(c)** Supposons maintenant que le pion se déplace à $v = 0.80c$ dans le labo et se désintègre en deux photons émis le long de l'axe de mouvement (un vers l'avant, un vers l'arrière). En utilisant la conservation de l'énergie totale et de l'impulsion totale dans le référentiel du labo, trouvez l'énergie de chacun des deux photons.

<details>
<summary><strong>Indice stratégique</strong></summary>
En (a), la quantité de mouvement totale initiale est nulle — qu'est-ce que ça impose aux photons ? En (b), essayez de satisfaire les deux lois de conservation en même temps : vous allez obtenir une contradiction. En (c), vous avez deux inconnues ($E_1$ et $E_2$) et deux équations (conservation de $E$ et de $p$). Pensez à calculer l'énergie totale et l'impulsion totale du pion dans le labo avant de commencer.

</details>
<details>
<summary><strong>Solution</strong></summary>
**(a)** Dans le référentiel de repos du pion, $\vec{p}_{\text{total, initial}} = 0$. Donc :

$$\vec{p}_{\gamma_1} + \vec{p}_{\gamma_2} = 0 \implies |\vec{p}_{\gamma_1}| = |\vec{p}_{\gamma_2}|$$

Les photons partent dans des directions **opposées** avec des impulsions de même module. Puisque $E = pc$ pour un photon, ils ont la même énergie :

$$2E_\gamma = m_\pi c^2 \implies E_\gamma = \frac{135.0}{2} = 67.5 \text{ MeV}$$

**(b)** Pion au repos → $\vec{p}_{\text{initial}} = 0$.

Conservation de l'impulsion pour un seul photon produit :

$$\vec{p}_\gamma = 0 \implies p_\gamma = 0$$

Mais un photon avec $p = 0$ a une énergie $E = pc = 0$. Or la conservation de l'énergie exige :

$$E_\gamma = m_\pi c^2 = 135.0 \text{ MeV} \neq 0$$

**Contradiction.** On ne peut pas satisfaire les deux lois simultanément. La désintégration en un seul photon est interdite — il faut au minimum deux photons.

**(c)** Avec $v = 0.80c$ : $\gamma = 5/3$, $\beta = 0.80$.

Énergie et impulsion du pion dans le labo :

$$E_\pi = \gamma m_\pi c^2 = \frac{5}{3} \times 135.0 = 225.0 \text{ MeV}$$

$$p_\pi c = \gamma m_\pi c^2 \times \beta = 225.0 \times 0.80 = 180.0 \text{ MeV}$$

Notons $E_1$ l'énergie du photon vers l'avant et $E_2$ celle du photon vers l'arrière. Pour chaque photon, $p = E/c$, avec un signe $+$ vers l'avant et $-$ vers l'arrière.

Conservation de l'énergie :

$$E_1 + E_2 = 225.0 \text{ MeV} \quad (1)$$

Conservation de l'impulsion (en multipliant par $c$) :

$$E_1 - E_2 = 180.0 \text{ MeV} \quad (2)$$

En additionnant (1) et (2) : $2E_1 = 405.0$, donc $E_1 = 202.5 \text{ MeV}$.

En soustrayant (2) de (1) : $2E_2 = 45.0$, donc $E_2 = 22.5 \text{ MeV}$.

**Vérification :** $E_1 + E_2 = 225.0$ ✓ et $E_1 - E_2 = 180.0$ ✓

Le photon vers l'avant emporte **9 fois** plus d'énergie que celui vers l'arrière — un effet dramatique du mouvement relativiste du pion.

</details>


## Exercice 4 — Gymnastique algébrique : énergie-impulsion (sans valeurs numériques)

> Tout est symbolique. L'objectif est de maîtriser les manipulations de la relation
> $E^2 = (pc)^2 + (mc^2)^2$ et de la conservation énergie-impulsion dans les désintégrations.


### Partie A — Identités utiles de la relation énergie-impulsion

La relation fondamentale pour une particule de masse $m$ est :

$$E^2 = (pc)^2 + (mc^2)^2$$

On rappelle aussi que $p = \gamma m v$ et $E = \gamma mc^2$.

**(a)** Montrez que pour toute particule massive :

$$\frac{v}{c} = \frac{pc}{E}$$

**(b)** Montrez que $\gamma = \dfrac{E}{mc^2}$. En déduire que l'énergie cinétique est :

$$E_k = (\gamma - 1)\,mc^2$$

<details>
<summary><strong>Solution partie A</strong></summary>

**(a)**

$$\frac{p}{E} = \frac{\gamma m v}{\gamma mc^2} = \frac{v}{c^2} \implies \frac{pc}{E} = \frac{v}{c}$$

> **Piège courant :** Les étudiants tentent de dériver cette relation à partir de $E^2 = (pc)^2 + (mc^2)^2$ en isolant $p$, ce qui donne $p = \frac{1}{c}\sqrt{E^2 - (mc^2)^2}$ — correct mais inutilement compliqué. La relation $v/c = pc/E$ est **directe** et doit être connue par cœur.

**(b)** De $E = \gamma mc^2$ :

$$\gamma = \frac{E}{mc^2}$$

L'énergie totale est la somme de l'énergie de masse et de l'énergie cinétique :

$$E = mc^2 + E_k \implies E_k = E - mc^2 = \gamma mc^2 - mc^2 = (\gamma - 1)\,mc^2$$

</details>

### Partie B — Limite non relativiste de $E_k$

**(c)** En utilisant le développement de Taylor $(1 - x)^{-1/2} \approx 1 + \frac{1}{2}x + \frac{3}{8}x^2 + \cdots$ avec $x = \beta^2$, développez $\gamma$ au deuxième ordre en $\beta$ et montrez que :

$$E_k \approx \frac{1}{2}mv^2 + \frac{3}{8}m\frac{v^4}{c^2} + \cdots$$

Identifiez le premier terme. Que représente le second ?

<details>
<summary><strong>Solution partie B</strong></summary>

$$\gamma = (1 - \beta^2)^{-1/2} \approx 1 + \frac{1}{2}\beta^2 + \frac{3}{8}\beta^4 + \cdots$$

$$E_k = (\gamma - 1)mc^2 \approx \left(\frac{1}{2}\beta^2 + \frac{3}{8}\beta^4\right)mc^2 = \frac{1}{2}m v^2 + \frac{3}{8}m\frac{v^4}{c^2} + \cdots$$

Le premier terme est l'**énergie cinétique classique** $\frac{1}{2}mv^2$.

Le second terme, $\frac{3}{8}\frac{mv^4}{c^2}$, est la **correction relativiste au premier ordre** — elle est négligeable tant que $v \ll c$, mais elle montre précisément à quel point l'approximation classique dévie.

> **Piège courant :** Les étudiants oublient que le développement de $(1-x)^{-1/2}$ donne $+\frac{1}{2}x$, pas $-\frac{1}{2}x$. L'exposant est $-1/2$, pas $+1/2$ ! C'est une erreur de signe extrêmement fréquente qui donne $E_k \approx -\frac{1}{2}mv^2$, un résultat absurde qu'ils ne remettent pas toujours en question.

</details>

### Partie C — Impulsion en fonction de l'énergie cinétique

**(d)** Soit une particule de masse $m$ et d'énergie cinétique $E_k$. En utilisant $E = E_k + mc^2$ et la relation énergie-impulsion, montrez que :

$$p = \frac{1}{c}\sqrt{E_k^2 + 2E_k\,mc^2}$$

puis factorisez sous la forme :

$$p = \frac{1}{c}\sqrt{E_k(E_k + 2mc^2)}$$

**(e)** Vérifiez les deux cas limites :

- **Non relativiste** ($E_k \ll mc^2$) : retrouvez $p \approx \sqrt{2mE_k}$
- **Ultra-relativiste** ($E_k \gg mc^2$) : retrouvez $p \approx E_k/c$

<details>
<summary><strong>Solution partie C</strong></summary>

**(d)**

$$E^2 = (pc)^2 + (mc^2)^2$$

$$(E_k + mc^2)^2 = (pc)^2 + (mc^2)^2$$

$$E_k^2 + 2E_k\,mc^2 + \cancel{(mc^2)^2} = (pc)^2 + \cancel{(mc^2)^2}$$

$$(pc)^2 = E_k^2 + 2E_k\,mc^2 = E_k(E_k + 2mc^2)$$

$$\boxed{p = \frac{1}{c}\sqrt{E_k(E_k + 2mc^2)}}$$

> **Piège courant :** L'erreur la plus fréquente est d'oublier le terme $2E_k\,mc^2$ lors du développement du carré $(E_k + mc^2)^2$. L'étudiant écrit $E_k^2 + (mc^2)^2$ au lieu de $E_k^2 + 2E_k\,mc^2 + (mc^2)^2$, et comme les $(mc^2)^2$ s'annulent, il obtient $p = E_k/c$ — le résultat ultra-relativiste ! — sans réaliser qu'il manque le terme dominant dans le régime non relativiste.

**(e)** Limite non relativiste ($E_k \ll mc^2$) :

$$E_k + 2mc^2 \approx 2mc^2$$

$$p \approx \frac{1}{c}\sqrt{E_k \cdot 2mc^2} = \frac{1}{c}\sqrt{2mE_k \cdot c^2} = \sqrt{2mE_k}$$

C'est la relation classique $E_k = \frac{p^2}{2m}$. ✓

Limite ultra-relativiste ($E_k \gg mc^2$) :

$$E_k + 2mc^2 \approx E_k$$

$$p \approx \frac{1}{c}\sqrt{E_k \cdot E_k} = \frac{E_k}{c}$$

On retrouve la relation d'un photon $E = pc$, ce qui est cohérent : à très haute énergie, la masse est négligeable. ✓

</details>

### Partie D — Désintégration à deux corps : formule générale

Une particule de masse $M$, **au repos**, se désintègre en deux particules de masses $m_1$ et $m_2$ (avec $M > m_1 + m_2$).

**(f)** Écrivez les deux équations de conservation (énergie et impulsion).

**(g)** En utilisant le fait que $|\vec{p}_1| = |\vec{p}_2| = p$ (conséquence de la conservation de l'impulsion), et la relation $E_i^2 = (pc)^2 + (m_i c^2)^2$ pour chaque particule, montrez que :

$$E_1^2 - E_2^2 = (m_1^2 - m_2^2)\,c^4$$

puis, en combinant avec $E_1 + E_2 = Mc^2$, déduisez :

$$\boxed{E_1 = \frac{(M^2 + m_1^2 - m_2^2)\,c^2}{2M}}$$

<details>
<summary><strong>Indice</strong></summary>

Vous avez deux expressions : $E_1^2 - E_2^2 = (m_1^2 - m_2^2)c^4$ et $E_1 + E_2 = Mc^2$. La première peut se factoriser en $(E_1 - E_2)(E_1 + E_2)$. Divisez pour trouver $E_1 - E_2$, puis résolvez le système.

</details>
<details>
<summary><strong>Solution partie D</strong></summary>

**(f)** Conservation de l'énergie :

$$Mc^2 = E_1 + E_2 \quad (1)$$

Conservation de l'impulsion (particule $M$ au repos → $\vec{p}_{\text{total}} = 0$) :

$$\vec{p}_1 + \vec{p}_2 = 0 \implies |\vec{p}_1| = |\vec{p}_2| = p$$

**(g)** Pour chaque particule :

$$E_1^2 = (pc)^2 + (m_1 c^2)^2 \qquad E_2^2 = (pc)^2 + (m_2 c^2)^2$$

Soustraction :

$$E_1^2 - E_2^2 = (m_1^2 - m_2^2)\,c^4 \quad (2)$$

Factorisation du membre de gauche :

$$(E_1 - E_2)(E_1 + E_2) = (m_1^2 - m_2^2)\,c^4$$

En utilisant (1) :

$$E_1 - E_2 = \frac{(m_1^2 - m_2^2)\,c^4}{Mc^2} = \frac{(m_1^2 - m_2^2)\,c^2}{M} \quad (3)$$

Addition de (1) et (3) :

$$2E_1 = Mc^2 + \frac{(m_1^2 - m_2^2)\,c^2}{M} = \frac{M^2 c^2 + (m_1^2 - m_2^2)\,c^2}{M}$$

$$\boxed{E_1 = \frac{(M^2 + m_1^2 - m_2^2)\,c^2}{2M}}$$

(et par symétrie $1 \leftrightarrow 2$ : $E_2 = \frac{(M^2 + m_2^2 - m_1^2)\,c^2}{2M}$)

> **Piège courant :** L'astuce clé est la **soustraction** $E_1^2 - E_2^2$ qui élimine $(pc)^2$. Un étudiant qui ne voit pas cette astuce essaie de résoudre un système de deux équations avec des carrés et des racines carrées — c'est algébriquement infernal et mène presque toujours à des erreurs. La factorisation en produit $(E_1 - E_2)(E_1 + E_2)$ est la « serrure » de tout le problème.

</details>

### Partie E — Vérifications et cas particuliers

**(h)** Vérifiez la formule de la partie D dans les cas particuliers suivants :

- **Désintégration symétrique** ($m_1 = m_2 = m$) : montrez que $E_1 = E_2 = \frac{Mc^2}{2}$.
- **Un produit sans masse** ($m_2 = 0$, par exemple un photon) : montrez que $E_1 = \frac{(M^2 + m_1^2)\,c^2}{2M}$ et $E_\gamma = \frac{(M^2 - m_1^2)\,c^2}{2M}$.
**(i)** Pour le cas $m_2 = 0$, utilisez la formule pour calculer l'impulsion $p$ des deux produits et vérifiez que $E_\gamma = pc$ (comme il se doit pour un photon).

<details>
<summary><strong>Solution partie E</strong></summary>

**(h)** Cas symétrique ($m_1 = m_2$) :

$$E_1 = \frac{(M^2 + m^2 - m^2)\,c^2}{2M} = \frac{M^2 c^2}{2M} = \frac{Mc^2}{2}$$

Les deux particules se partagent l'énergie également. ✓ (C'est exactement le résultat du $\pi^0 \to \gamma\gamma$ de l'exercice 3 avec $m_1 = m_2 = 0$.)

Cas $m_2 = 0$ :

$$E_1 = \frac{(M^2 + m_1^2)\,c^2}{2M} \qquad E_\gamma = \frac{(M^2 - m_1^2)\,c^2}{2M}$$

Vérification : $E_1 + E_\gamma = \frac{(M^2 + m_1^2 + M^2 - m_1^2)\,c^2}{2M} = \frac{2M^2 c^2}{2M} = Mc^2$ ✓

**(i)** L'impulsion commune $p$ se trouve via $E_\gamma = pc$ (photon sans masse) :

$$pc = E_\gamma = \frac{(M^2 - m_1^2)\,c^2}{2M}$$

Vérifions avec la particule 1 :

$$E_1^2 - (pc)^2 = E_1^2 - E_\gamma^2 = (E_1 - E_\gamma)(E_1 + E_\gamma)$$

$$= \frac{2m_1^2\,c^2}{2M} \cdot Mc^2 = m_1^2\,c^4$$

Donc $E_1^2 - (pc)^2 = (m_1 c^2)^2$, ce qui est bien la relation énergie-impulsion pour une particule de masse $m_1$. ✓

> **Piège courant :** En (i), les étudiants vérifient souvent $E_\gamma = pc$ en recalculant $p$ à partir de la particule 1 via $p = \frac{1}{c}\sqrt{E_1^2 - (m_1 c^2)^2}$, ce qui est correct mais demande de développer $(M^2 + m_1^2)^2 - (2Mm_1)^2$. On reconnaît une **différence de carrés** : $(M^2 + m_1^2 - 2Mm_1)(M^2 + m_1^2 + 2Mm_1) = (M - m_1)^2(M + m_1)^2$. L'étudiant qui ne voit pas cette factorisation se perd dans un développement de 4+ termes.

</details>
