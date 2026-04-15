# Sujet 2 — Relativité restreinte : masse-énergie, fission nucléaire, désintégration

> **Objectif :** Savoir naviguer entre énergie de masse, énergie cinétique et énergie totale,
> et appliquer la conservation de l'énergie-impulsion à des processus nucléaires et de désintégration.

## Exercice 1 — Le prix d'un café

On chauffe une tasse de café (masse d'eau $m = 250 \text{ g}$) de $20°\text{C}$ à $80°\text{C}$.

Données : $c_{\text{eau}} = 4.18 \text{ J/(g·°C)}$

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

## Exercice 3 — Désintégration interdite ?

Un pion neutre ($\pi^0$) au repos se désintègre en deux photons :

$$\pi^0 \;\longrightarrow\; \gamma + \gamma$$

Masse du pion : $m_{\pi} = 135.0 \text{ MeV}/c^2$

**(a)** Par conservation de l'énergie-impulsion, trouvez l'énergie de chaque photon dans le référentiel de repos du pion.

**(b)** Un étudiant propose la désintégration en un **seul** photon : $\pi^0 \to \gamma$. Montrez que c'est impossible en utilisant la conservation du quadri-impulsion ($p^\mu p_\mu = \text{invariant}$).

**(c)** Un pion $\pi^0$ se déplace à $v = 0.80c$ dans le référentiel du labo et se désintègre en deux photons émis le long de l'axe de mouvement (un vers l'avant, un vers l'arrière). Trouvez l'énergie de chacun des deux photons dans le référentiel du labo.

<details>
<summary><strong>Indice stratégique</strong></summary>

En (a), exploitez la symétrie du problème dans le référentiel de repos. En (b), calculez l'invariant $p^\mu p_\mu$ avant et après — pour un photon, cet invariant vaut toujours zéro. En (c), utilisez la transformation de Lorentz sur les composantes de la quadri-impulsion des photons, ou bien travaillez directement avec conservation de $E$ et $p$ dans le labo.

</details>

<details>
<summary><strong>Solution</strong></summary>

**(a)** Dans le référentiel de repos du pion, la quantité de mouvement totale est nulle. Les deux photons doivent partir dans des directions opposées avec des impulsions égales en module, donc des énergies égales :

$$2E_\gamma = m_\pi c^2 \implies E_\gamma = \frac{135.0}{2} = 67.5 \text{ MeV}$$

**(b)** Invariant avant la désintégration (pion au repos) :

$$p^\mu p_\mu = (m_\pi c)^2 > 0$$

Invariant après la désintégration (un seul photon) :

$$p^\mu p_\mu = 0 \quad \text{(masse nulle du photon)}$$

Or $p^\mu p_\mu$ est un invariant de Lorentz : il doit être le même avant et après. On obtient $(m_\pi c)^2 = 0$, ce qui est une contradiction. **La désintégration en un seul photon est interdite.** Il faut au minimum deux photons pour satisfaire simultanément conservation de l'énergie et de l'impulsion.

**(c)** Avec $v = 0.80c$, on a $\gamma = 5/3$ et $\beta = 0.80$.

**Méthode — transformation de Lorentz des quadri-impulsions :**

Dans le référentiel de repos, les deux photons ont :
- Photon avant : $E^* = 67.5 \text{ MeV}$, $p^*c = +67.5 \text{ MeV}$
- Photon arrière : $E^* = 67.5 \text{ MeV}$, $p^*c = -67.5 \text{ MeV}$

Transformation vers le labo ($E = \gamma(E^* + v\,p^*)$) :

$$E_{\text{avant}} = \gamma(E^* + \beta\,p^*c) = \frac{5}{3}(67.5 + 0.80 \times 67.5) = \frac{5}{3} \times 121.5 = 202.5 \text{ MeV}$$

$$E_{\text{arrière}} = \gamma(E^* - \beta\,p^*c) = \frac{5}{3}(67.5 - 0.80 \times 67.5) = \frac{5}{3} \times 13.5 = 22.5 \text{ MeV}$$

**Vérification :** $E_{\text{avant}} + E_{\text{arrière}} = 225 \text{ MeV} = \gamma m_\pi c^2 = \frac{5}{3} \times 135$ ✓

Le photon émis vers l'avant est boosté à $202.5 \text{ MeV}$, celui vers l'arrière est réduit à $22.5 \text{ MeV}$ — un rapport de 9:1, illustration spectaculaire de l'effet Doppler relativiste.

</details>
