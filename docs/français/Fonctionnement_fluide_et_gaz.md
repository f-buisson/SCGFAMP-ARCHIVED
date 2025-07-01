
# 🔬 Fonctionnement biomimétique – Déplacement des fluides et gaz

Ce système s’inspire d’un **poumon mécanique**, non pas pour reproduire un organe biologique, mais pour **imiter sa logique de fonctionnement cyclique passif**.  
Il repose sur des différences de pression, la compressibilité de l’air, la gravité, et des trappes unidirectionnelles.

---

## 🫁 1. Inspiration

- Lorsque la pression dans la colonne d’air descend en dessous d’un seuil critique (par exemple < 0,7 bar), une **entrée d’air atmosphérique (1 bar)** s’ouvre automatiquement.
- L’air entre alors dans la colonne d’air, ce qui :
  - régule la pression interne (vers 1 bar),
  - permet d’amorcer un **déplacement du surplus d’eau** présent dans cette colonne (à cause du passage d’eau via les trappes depuis la colonne d’eau).
- Ce retour à pression atmosphérique facilite le **refoulement de l’eau** dans la colonne d’eau (via des clapets).

🔁 Cette phase joue le rôle d’une “inspiration” dans un système respiratoire : entrée d’air = régulation = mouvement de fluide.

---

## 🌬️ 2. Expiration

- Lors de la phase précédente, de l’eau est entrée dans la colonne d’air → **elle occupe une partie du volume initialement rempli par l’air**.
- Comme l’air est compressible, il **ne se fait pas expulser**, mais **se réorganise naturellement** :
  - Il se **repartit** vers les volumes disponibles — dont une partie peut être la **colonne d’eau reliée** à celle d’air.
  - Cette redistribution se fait sans pompe : elle résulte d’un **équilibre de volume et de pression**.
- L’air ainsi déplacé vers la colonne d’eau est ensuite **évacué via un purgeur**, ce qui :
  - abaisse la pression dans cette colonne,
  - crée une **dépression utile pour attirer l’eau** dans la phase suivante.

🔁 Cette phase équivaut à une “expiration” : l’air excédentaire est purgé, et un vide utile est préparé.

---

## 🔁 Résumé du cycle passif

1. **Dépression** dans la colonne d’air → air extérieur entre
2. L’air régule la pression et **refoule l’eau** vers sa colonne d’origine
3. L’eau **revient dans la colonne d’air** (via trappes) → l’air se compresse
4. Une partie de l’air **se répartit vers la colonne d’eau** (effet de volume)
5. L’air est **purgé**, générant une **nouvelle dépression**
6. La dépression aide à **réattirer l’eau dans la colonne d’eau**
7. 🔄 Le cycle recommence

---

## 📌 Note technique

Ce système ne contient :
- ni moteur
- ni pompe
- ni action mécanique active

Il repose sur :
- les lois de la pression et de la compressibilité des gaz,
- la gravité et la flottabilité des fluides,
- un jeu de trappes unidirectionnelles pour orienter les flux.

⚠️ Le comportement réel dépendra fortement :
- des volumes,
- de la géométrie,
- du timing de chaque phase,
- de l’étanchéité du système.

---

## 🧠 But du projet

Le système n’est **pas présenté comme un dispositif énergétique autonome**, mais comme un **prototype expérimental** :  
> Un cycle gravito-flottant fluide passif, inspiré de la respiration naturelle, à étudier, tester, corriger.
