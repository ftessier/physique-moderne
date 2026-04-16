# Guide d'amorce — PHY 2761

## Le problème que tu vis (et que tout le monde vit)

Tu lis la question. Tu comprends de quoi ça parle. Tu sais même quelle équation utiliser. Mais tu restes planté devant ta feuille parce que tu ne sais pas **par quel bout commencer le calcul**. C'est normal : les équations sur la feuille de formules sont des outils, mais personne ne t'a montré la procédure pour **choisir lequel prendre en premier** et **dans quel sens le tourner**.

Ce guide te donne un rituel en 3 gestes à faire *systématiquement* avant d'écrire la moindre équation. Ensuite, pour chaque type de problème de l'examen, on détaille exactement l'amorce — les 30 premières secondes.

## Conventions de notation

Dans tout ce document :

- $L$ = longueur mesurée par un observateur qui voit l'objet en mouvement
- $L_0$ = longueur propre (mesurée au repos par rapport à l'objet)
- $v_A$, $v_B$ = vitesses des navettes dans le référentiel de l'observateur fixe
- $v_{A/B}$ = vitesse de A mesurée dans le référentiel de B
- $\gamma$ = facteur de Lorentz, $\gamma = 1/\sqrt{1 - v^2/c^2}$, toujours $\geq 1$
- $\beta = v/c$
- $K$ = énergie cinétique
- $\phi$ = travail de seuil (effet photoélectrique)
- $\theta$ = angle de diffusion du photon (Compton)
- $\varphi$ = angle de recul de l'électron (Compton)
- $\lambda_C = h/(m_e c) = 0{,}00243\;\text{nm}$ = longueur d'onde Compton de l'électron
- $E_n$ = énergie du niveau $n$ de l'hydrogène
- $\Psi(x)$ = fonction d'onde
- $\hat{A}$ = opérateur associé à l'observable $A$


## Le rituel universel (3 gestes, toujours les mêmes)

### Geste 1 — Inventaire

Prends 15 secondes. Écris deux colonnes sur ta feuille :

| DONNÉ | CHERCHÉ |
| ----- | ------- |
| ...   | ...     |

Écris **tout** ce qui est donné, **avec les unités et les signes**. Tu ne réfléchis pas encore. Tu recopies. Si une vitesse va vers la gauche, mets le signe négatif tout de suite. Si c'est une longueur « mesurée par un observateur fixe », note-le. **C'est la mise en scène du problème.**

> Pourquoi ça marche : 80 % du temps, l'amorce devient évidente une fois l'inventaire posé. Tu vois ce que tu as, tu vois ce qu'il te manque, et une seule équation fait le pont.

### Geste 2 — Le pont

Regarde la colonne CHERCHÉ. Regarde ta feuille de formules. Cherche l'équation qui **contient la quantité cherchée** et dont **toutes les autres variables sont dans la colonne DONNÉ** (ou calculables facilement à partir du donné). C'est ton équation de pont.

> Si tu trouves pas de pont direct : c'est qu'il y a une **quantité intermédiaire** à calculer d'abord. Ajoute-la dans la colonne CHERCHÉ, en première position, et recommence le Geste 2 avec elle.

### Geste 3 — Isoler avant de calculer

Avant de toucher ta calculatrice : **isole algébriquement la variable cherchée**. Tu ne substitues les chiffres qu'à la toute fin. Ça t'évite les erreurs de frappe et ça te permet de vérifier les unités.


## Application à chaque problème de l'examen


### Problème 1 — Relativité restreinte (navettes)

**Contexte général :** Deux navettes, un observateur fixe, des vitesses relativistes. C'est un problème multi-référentiels.

**Réflexe spécifique à la relativité :** Avant même l'inventaire, pose-toi LA question : **« Qui mesure quoi, dans quel référentiel ? »** Note le référentiel à côté de chaque donnée. C'est ça, l'étape invisible que l'expérience t'apprend.

#### 1a — Longueurs propres

**Inventaire :**

| DONNÉ                                       | CHERCHÉ                          |
| ------------------------------------------- | -------------------------------- |
| $L_A = 30\;\text{m}$ (mesuré par obs. fixe) | $L_{0,A}$ (longueur propre de A) |
| $L_B = 30\;\text{m}$ (mesuré par obs. fixe) | $L_{0,B}$ (longueur propre de B) |
| $v_A = 0{,}65\,c$                           |                                  |
| $v_B = 0{,}85\,c$                           |                                  |

**Le pont :** La formule de contraction des longueurs relie $L$ à $L_0$ :

$$L = \frac{L_0}{\gamma}$$

Tu as $L$, tu peux calculer $\gamma$ avec $v$. Donc tu peux isoler $L_0$.

**L'amorce concrète :**

1. Calcule $\gamma_A = \dfrac{1}{\sqrt{1 - (0{,}65)^2}}$

2. Isole : $L_{0,A} = \gamma_A \cdot L_A$

3. Même chose pour B avec $\gamma_B$.

> **Le piège classique :** Se tromper de sens dans $L = L_0/\gamma$. Rappelle-toi : la longueur mesurée par quelqu'un qui voit l'objet bouger est **toujours plus courte**. Donc $L_0 > L$, donc $L_0 = \gamma L$ (puisque $\gamma > 1$).

#### 1b — Longueur de A vue par B (et vice versa)

**Pourquoi c'est plus dur :** Ici, ni A ni B n'est l'observateur fixe. Il faut d'abord trouver la vitesse de A **dans le référentiel de B**.

**L'amorce :**

1. **Quantité intermédiaire** $\rightarrow$ vitesse relative $v_{A/B}$ (vitesse de A vue par B)

2. Loi d'addition relativiste des vitesses :

$$v'_x = \frac{v_x - v}{1 - \dfrac{v_x \, v}{c^2}}$$

3. Ici $v_x = v_A = +0{,}65\,c$ et $v = v_B = -0{,}85\,c$ (B est le nouveau référentiel)

4. Une fois $v_{A/B}$ trouvée, calcule $\gamma_{A/B}$

5. Puis : $L_{A \text{ vu par } B} = \dfrac{L_{0,A}}{\gamma_{A/B}}$

> **Le piège :** Les signes dans l'addition des vitesses. Fais un petit dessin avec des flèches. Si elles vont en sens contraire, la vitesse relative sera très grande (proche de $c$, mais jamais au-dessus).

#### 1c — Temps avant collision (observateur fixe)

**Inventaire :**

| DONNÉ                              | CHERCHÉ                     |
| ---------------------------------- | --------------------------- |
| $d = 5 \times 10^{12}\;\text{m}$   | $t$ (temps avant collision) |
| $v_A = 0{,}65\,c$ (vers la droite) |                             |
| $v_B = 0{,}85\,c$ (vers la gauche) |                             |

**Le pont :** C'est de la cinématique de base. Les deux navettes se rapprochent, donc la vitesse de rapprochement est $v_A + |v_B|$ (attention : ici, **PAS** d'addition relativiste parce qu'on reste dans un seul référentiel, celui de l'observateur fixe).

**L'amorce :**

1. Vitesse de rapprochement : $v_A + |v_B| = 0{,}65\,c + 0{,}85\,c = 1{,}50\,c$

2. Temps :

$$t = \frac{d}{v_A + |v_B|}$$

> **Le piège :** Vouloir utiliser l'addition relativiste ici. L'addition relativiste sert à **changer de référentiel**. Ici, on reste dans le même référentiel. Deux objets peuvent se rapprocher à plus de $c$ dans un référentiel donné — c'est leur vitesse relative *dans le référentiel de l'un d'eux* qui ne peut pas dépasser $c$.

#### 1d — Temps avant collision selon les pilotes

**L'amorce :**

1. Tu as trouvé $t$ au 1c (temps dans le référentiel fixe).

2. Pour le pilote A (dilatation du temps) :

$$\Delta t_A = \frac{t}{\gamma_A}$$

3. Pour le pilote B :

$$\Delta t_B = \frac{t}{\gamma_B}$$

> **Le piège :** Le sens de la dilatation. Le temps propre (mesuré par celui qui « vit » l'événement au même endroit) est **toujours le plus court**. Le pilote voit la collision arriver plus vite.

#### 1e — Longueurs d'onde (effet Doppler relativiste)

**L'amorce :**

1. Identifie si la source et l'observateur se rapprochent ou s'éloignent.

2. Source fixe, laser émis en direction $\hat{x}$ :
   - A se déplace dans le sens du laser $\rightarrow$ **s'éloigne** de la source $\rightarrow$ décalage vers le rouge
   - B se déplace en sens opposé $\rightarrow$ **se rapproche** $\rightarrow$ décalage vers le bleu

3. Formule Doppler relativiste (s'éloigne) :

$$\lambda' = \lambda_0 \sqrt{\frac{1 + \beta}{1 - \beta}}$$

4. Formule Doppler relativiste (se rapproche) :

$$\lambda' = \lambda_0 \sqrt{\frac{1 - \beta}{1 + \beta}}$$

5. Vérification du sens physique : s'éloigne $\Rightarrow$ $\lambda' > \lambda_0$, se rapproche $\Rightarrow$ $\lambda' < \lambda_0$.

> **Le piège :** Oublier de vérifier le sens physique du résultat. Si tu t'éloignes d'un laser rouge, tu dois mesurer une longueur d'onde **plus grande** (plus rouge, voire infrarouge).


### Problème 2 — Effet photoélectrique

**Inventaire :**

| DONNÉ                                                                                    | CHERCHÉ                   |
| ---------------------------------------------------------------------------------------- | ------------------------- |
| Source 1 : longueur d'onde $\lambda$ $\;\rightarrow\;$ $K_{\max,1} = 2{,}5\;\text{eV}$   | $\phi$ (travail de seuil) |
| Source 2 : longueur d'onde $\lambda/2$ $\;\rightarrow\;$ $K_{\max,2} = 7{,}0\;\text{eV}$ |                           |

**Le pont :** L'équation photoélectrique :

$$K_{\max} = \frac{hc}{\lambda} - \phi$$

**L'amorce :**

1. Écris l'équation **deux fois**, une pour chaque source :

$$(1)\quad 2{,}5 = \frac{hc}{\lambda} - \phi$$

$$(2)\quad 7{,}0 = \frac{hc}{\lambda/2} - \phi = \frac{2hc}{\lambda} - \phi$$

2. Tu as maintenant un **système de 2 équations à 2 inconnues** ($hc/\lambda$ et $\phi$).

3. Soustrais $(1)$ de $(2)$ :

$$7{,}0 - 2{,}5 = \frac{2hc}{\lambda} - \frac{hc}{\lambda} \quad\Longrightarrow\quad \frac{hc}{\lambda} = 4{,}5\;\text{eV}$$

4. Substitue dans $(1)$ : $\phi = 4{,}5 - 2{,}5 = 2{,}0\;\text{eV}$

> **La leçon :** Quand tu as deux situations expérimentales et une inconnue commune, **écris la même équation deux fois** et fais un système. C'est un patron récurrent en physique.


### Problème 3 — Diffusion Compton

**Inventaire :**

| DONNÉ                                                                | CHERCHÉ                                           |
| -------------------------------------------------------------------- | ------------------------------------------------- |
| $E_i = 120 \times 10^{4}\;\text{eV}$ (énergie initiale du photon)    | a) $\lambda'$ (longueur d'onde du photon diffusé) |
| $K_e = 40 \times 10^{4}\;\text{eV}$ (énergie de recul de l'électron) | b) $\theta$ (angle de diffusion du photon)        |
|                                                                      | c) $\varphi$ (angle de recul de l'électron)       |

#### 3a — Longueur d'onde du photon diffusé

**L'amorce :**

1. Conservation de l'énergie $\rightarrow$ énergie du photon diffusé :

$$E_f = E_i - K_e = 80 \times 10^{4}\;\text{eV}$$

2. Conversion énergie $\rightarrow$ longueur d'onde via $E = hc/\lambda$ :

$$\lambda' = \frac{hc}{E_f}$$

3. Substitue (utilise $hc = 1240\;\text{eV}\!\cdot\!\text{nm}$ pour un calcul rapide).

> **L'astuce unités :** $hc = 1240\;\text{eV}\!\cdot\!\text{nm}$. Si $E$ est en eV, alors $\lambda\;(\text{en nm}) = 1240 / E\;(\text{en eV})$. Mémorise ce nombre, il fait gagner du temps.

#### 3b — Angle de diffusion $\theta$

**L'amorce :**

1. Tu connais maintenant $\lambda$ et $\lambda'$. La formule de Compton les relie à $\theta$ :

$$\lambda' - \lambda = \lambda_C\,(1 - \cos\theta)$$

où $\lambda_C = h/(m_e c) = 0{,}00243\;\text{nm}$.

2. Calcule $\Delta\lambda = \lambda' - \lambda$

3. Isole :

$$\cos\theta = 1 - \frac{\Delta\lambda}{\lambda_C}$$

4. $\theta = \arccos(\ldots)$

#### 3c — Angle de recul $\varphi$ de l'électron

**L'amorce :**

1. Conservation de la quantité de mouvement en 2D (composantes $x$ et $y$) :

$$p_i = p_f \cos\theta + p_e \cos\varphi \qquad\text{(composante }x\text{)}$$

$$0 = p_f \sin\theta - p_e \sin\varphi \qquad\text{(composante }y\text{)}$$

2. Pour les photons : $p = E/c$, donc $p_i = E_i/c$ et $p_f = E_f/c$.

3. Pour l'électron (relativiste), utilise la relation énergie-impulsion :

$$E_{\text{tot}}^2 = (p_e c)^2 + (m_e c^2)^2$$

avec $E_{\text{tot}} = K_e + m_e c^2$, pour trouver $p_e$.

4. Tu connais $\theta$ (du 3b) et toutes les impulsions $\rightarrow$ isole $\varphi$.

> **Le piège :** La quantité de mouvement de l'électron n'est **PAS** $p_e = m_e v$ ici (vitesses relativistes). Utilise toujours $E^2 = (pc)^2 + (mc^2)^2$.


### Problème 4 — Atome d'hydrogène

**Réflexe pour tout problème d'hydrogène :** L'énergie du niveau $n$ est :

$$E_n = -\frac{13{,}6}{n^2}\;\text{eV}$$

**Écris-la immédiatement** pour les niveaux concernés.

#### 4a — Énergie d'ionisation depuis $n = 15$

**L'amorce :**

1. Énergie d'ionisation = énergie pour amener l'électron de $n = 15$ à $n = \infty$ :

$$E_{\text{ion}} = E_\infty - E_{15} = 0 - \left(-\frac{13{,}6}{15^2}\right) = \frac{13{,}6}{225}\;\text{eV}$$

C'est tout. Un seul calcul.

#### 4b — Fréquence du photon émis ($n = 15 \to n = 5$)

**L'amorce :**

1. Différence d'énergie entre les niveaux :

$$\Delta E = E_{15} - E_5 = \left(-\frac{13{,}6}{225}\right) - \left(-\frac{13{,}6}{25}\right)$$

2. Énergie du photon émis :

$$E_\gamma = |\Delta E|$$

3. Fréquence :

$$f = \frac{E_\gamma}{h}$$

> **Le piège :** Les signes. $E_{15}$ est moins négatif que $E_5$ (plus haut en énergie sur le diagramme). Le photon est émis, donc $\Delta E < 0$. L'énergie du photon est la valeur absolue.

#### 4c — Recul de l'atome

**L'amorce :**

1. Conservation de la quantité de mouvement : avant l'émission, tout est au repos $\Rightarrow$ $\vec{p}_{\text{total}} = \vec{0}$.

2. Après l'émission :

$$\vec{p}_\gamma + \vec{p}_{\text{atome}} = \vec{0} \qquad\Longrightarrow\qquad p_{\text{atome}} = p_\gamma$$

3. Impulsion du photon :

$$p_\gamma = \frac{E_\gamma}{c}$$

4. Énergie cinétique de recul (atome non relativiste, masse $m_H$) :

$$K_{\text{recul}} = \frac{p_{\text{atome}}^2}{2\,m_H}$$

> C'est un problème de conservation. Dès que tu vois « recul », pense **conservation de $\vec{p}$**.

#### 4d — Largeur de raie

**L'amorce :**

1. Principe d'incertitude énergie-temps :

$$\Delta E \cdot \Delta t \geq \frac{\hbar}{2}$$

2. Chaque niveau a une durée de vie finie $\rightarrow$ chacun contribue une incertitude en énergie :

$$\Delta E_{\text{total}} \approx \frac{\hbar}{\tau_{15}} + \frac{\hbar}{\tau_5}$$

3. Largeur de raie en fréquence :

$$\Delta f = \frac{\Delta E_{\text{total}}}{h} = \frac{1}{2\pi}\left(\frac{1}{\tau_{15}} + \frac{1}{\tau_5}\right)$$

> **Le patron :** Dès que tu vois « largeur de raie » ou « durée de vie », c'est le principe d'incertitude $\Delta E \cdot \Delta t$.


### Problème 5 — Puits de potentiel infini

#### 5a — Équation de Schrödinger

**L'amorce :** C'est sur ta feuille de formules. À l'intérieur du puits, $V(x) = 0$ :

$$-\frac{\hbar^2}{2m}\,\frac{d^2\Psi(x)}{dx^2} = E\,\Psi(x)$$

Écris-la, c'est tout. Pas de calcul ici.

#### 5b — Vérifier que $\Psi(x) = A\sin\!\left(\dfrac{n\pi x}{L}\right)$ est solution

**L'amorce :**

1. Substitue $\Psi$ dans le côté gauche de l'équation.

2. Dérive $\sin\!\left(\dfrac{n\pi x}{L}\right)$ deux fois :

$$\frac{d^2}{dx^2}\sin\!\left(\frac{n\pi x}{L}\right) = -\left(\frac{n\pi}{L}\right)^2 \sin\!\left(\frac{n\pi x}{L}\right)$$

3. Substitue dans l'équation de Schrödinger :

$$-\frac{\hbar^2}{2m}\left[-\left(\frac{n\pi}{L}\right)^2\right]\Psi(x) = \frac{\hbar^2 n^2 \pi^2}{2mL^2}\,\Psi(x)$$

4. Le résultat est bien de la forme $E\,\Psi(x)$, ce qui donne en bonus :

$$E_n = \frac{\hbar^2 n^2 \pi^2}{2mL^2}$$

> **Le patron « montrer que » :** Tu pars toujours du côté le plus compliqué et tu montres qu'il se réduit à l'autre côté. Ici : côté gauche $\rightarrow$ substitue $\rightarrow$ simplifie $\rightarrow$ côté droit.

#### 5c — Position moyenne $\langle x \rangle$

**L'amorce :**

1. Formule de la valeur moyenne :

$$\langle x \rangle = \int_0^L \Psi^*(x)\, x\, \Psi(x)\, dx$$

2. Avec $\Psi(x) = A\sin\!\left(\dfrac{n\pi x}{L}\right)$ :

$$\langle x \rangle = A^2 \int_0^L x\,\sin^2\!\left(\frac{n\pi x}{L}\right) dx$$

3. Utilise l'identité $\sin^2 u = \dfrac{1 - \cos 2u}{2}$ pour séparer l'intégrale.

> **Le piège :** Oublier la normalisation (trouver $A^2$ d'abord, ou vérifier que $A = \sqrt{2/L}$ ).

#### 5d — Position la plus probable ($n = 2$)

**L'amorce :**

1. La position la plus probable maximise $|\Psi|^2$, donc maximise $\sin^2\!\left(\dfrac{2\pi x}{L}\right)$.

2. $\sin^2$ est maximal quand $\sin = \pm 1$, donc :

$$\frac{2\pi x}{L} = \frac{\pi}{2},\;\frac{3\pi}{2},\;\ldots$$

3. Solutions :

$$x = \frac{L}{4} \qquad\text{et}\qquad x = \frac{3L}{4}$$

> Pour $n = 2$, il y a **deux** maxima (le nœud au milieu à $x = L/2$ sépare deux bosses).

#### 5e — Énergie cinétique moyenne ($n = 2$)

**L'amorce :**

1. En principe :

$$\langle \hat{T} \rangle = \int_0^L \Psi^*(x)\left(-\frac{\hbar^2}{2m}\,\frac{d^2}{dx^2}\right)\Psi(x)\,dx$$

2. Mais dans le puits infini avec $V = 0$ : $\hat{T}\,\Psi = E\,\Psi$.

3. Donc **pas d'intégrale à calculer** :

$$\langle \hat{T} \rangle = E_2 = \frac{4\,\hbar^2\pi^2}{2mL^2}$$

> **Le raccourci :** Si $V = 0$ dans tout le puits, toute l'énergie est cinétique. $\langle \hat{T} \rangle = E_n$, point final.

#### 5f — Quantité de mouvement moyenne ($n = 2$)

**L'amorce :**

1. Opérateur impulsion :

$$\langle \hat{p} \rangle = \int_0^L \Psi^*(x)\left(-i\hbar\,\frac{d}{dx}\right)\Psi(x)\,dx$$

2. La dérivée donne :

$$\frac{d}{dx}\sin\!\left(\frac{2\pi x}{L}\right) = \frac{2\pi}{L}\cos\!\left(\frac{2\pi x}{L}\right)$$

3. L'intégrale contient $\sin\!\left(\dfrac{2\pi x}{L}\right)\cos\!\left(\dfrac{2\pi x}{L}\right) = \dfrac{1}{2}\sin\!\left(\dfrac{4\pi x}{L}\right)$, intégrée sur une période complète :

$$\langle \hat{p} \rangle = 0$$

> **Le sens physique :** L'électron dans un puits n'a pas de direction privilégiée (autant de chances d'aller à gauche qu'à droite). Donc $\langle \hat{p} \rangle = 0$, toujours. Si tu arrives à autre chose, c'est une erreur.


### Problème 6 — Proton dans un champ magnétique

**Inventaire :**

| DONNÉ                           | CHERCHÉ                            |
| ------------------------------- | ---------------------------------- |
| Mouvement circulaire, rayon $R$ | $p = 300\,B\,R$                    |
| Champ magnétique $B$            | (en $\text{MeV}/c$, Tesla, mètres) |

**L'amorce :**

1. Force magnétique = force centripète. Comme $p = \gamma m v$ :

$$qvB = \frac{pv}{R}$$

2. Les $v$ se simplifient :

$$p = qBR$$

3. Substitue $q = 1{,}602 \times 10^{-19}\;\text{C}$ et convertis en $\text{MeV}/c$ :

$$p\;\left[\frac{\text{MeV}}{c}\right] = \frac{q \cdot B \cdot R}{\dfrac{1{,}602 \times 10^{-13}\;\text{J}}{3 \times 10^{8}\;\text{m/s}}} = \frac{1{,}602 \times 10^{-19} \times 3 \times 10^{8}}{1{,}602 \times 10^{-13}}\;BR = 300\,BR$$

> **L'astuce :** L'équation $p = qBR$ est **exacte en relativité** (pas besoin de connaître $\gamma$). C'est pourquoi on l'utilise en physique des particules. Le problème est essentiellement un exercice de conversion d'unités.


### Problème 7 — Diffraction d'électrons

#### Partie 1 : Trouver la différence de potentiel

**L'amorce :**

1. On veut $\lambda = 1 \times 10^{-10}\;\text{m}$ pour les électrons.

2. De Broglie donne l'impulsion :

$$p = \frac{h}{\lambda}$$

3. L'énergie cinétique vient de l'accélération par une ddp $V$ :

$$K = eV$$

4. Relation $K$-$p$ (non relativiste, à vérifier a posteriori) :

$$K = \frac{p^2}{2m_e}$$

5. Combine et isole $V$ :

$$eV = \frac{h^2}{2m_e\lambda^2} \qquad\Longrightarrow\qquad V = \frac{h^2}{2m_e\, e\,\lambda^2}$$

#### Partie 2 : Distances interatomiques (loi de Bragg)

**L'amorce :**

1. Loi de Bragg (avec $n = 1$ pour le premier ordre) :

$$2d\sin\theta = \lambda$$

2. Isole $d$ :

$$d = \frac{\lambda}{2\sin\theta}$$

3. Calcule pour $\theta = 24°$ et $\theta = 51°$.


## Résumé — Les patrons récurrents

| Tu vois...                                           | Tu fais d'abord...                                                                                                |
| ---------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Plusieurs référentiels / vitesses                    | **Dessine** et étiquette chaque quantité avec son référentiel                                                     |
| « Longueur/temps mesuré par... »                     | Identifie $L_0$ / $\Delta t_0$ (propre) vs $L$ / $\Delta t$ (mesuré), applique $\gamma$ dans le bon sens          |
| Deux situations expérimentales, une inconnue commune | Écris la même équation **deux fois**, fais un système                                                             |
| Conservation (collision, émission, diffusion)        | Écris conservation de $E$ **et** conservation de $\vec{p}$ (composante par composante si 2D)                      |
| « Montrer que... »                                   | Pars du côté compliqué, substitue, simplifie vers le côté simple                                                  |
| Valeur moyenne $\langle \hat{A} \rangle$             | Écris $\int \Psi^* \hat{A}\, \Psi\, dx$, identifie l'opérateur                                                    |
| « Position la plus probable »                        | Dérive $                                                                                                          | \Psi | ^2$, égale à zéro |
| « Largeur de raie » ou « durée de vie »              | Principe d'incertitude $\Delta E \cdot \Delta t \geq \hbar/2$                                                     |
| Recul après émission                                 | Conservation de $\vec{p}$, système initialement au repos                                                          |
| Conversion d'unités                                  | $hc = 1240\;\text{eV}\!\cdot\!\text{nm}$, $\;m_e c^2 = 0{,}511\;\text{MeV}$, $\;\lambda_C = 0{,}00243\;\text{nm}$ |
| Force dans un champ $B$                              | Force magnétique = force centripète, $p = qBR$                                                                    |
| de Broglie + accélération                            | $\lambda = h/p$ et $K = eV$, combine via $K = p^2/(2m)$                                                           |


## Le mot de la fin

L'amorce n'est pas de l'inspiration — c'est un **algorithme** :

1. **Inventaire** (donné/cherché, avec référentiels et unités)
2. **Pont** (quelle équation contient le cherché avec le donné ?)
3. **Isoler** (algèbre d'abord, chiffres ensuite)

Si le pont n'est pas direct : cherche la **quantité intermédiaire** ($\gamma$, une vitesse relative, une énergie de photon...) et recommence le cycle avec elle.

Avec de la pratique, ces gestes deviennent automatiques. Tu ne « trouveras » plus l'amorce — tu la **construiras**, mécaniquement, à chaque fois.
