# FAQ – SCGFAMP (FR)

---

### « "Prise d’air depuis l’atmosphère", mais c’est une prise d’air vers une chambre d’air pressurisé. »

C’est une prise d’air vers une chambre d’air à vide partiel (entre 0,5 et 0,7 bar). Oui cela demande de l’énergie au départ pour créer ce déséquilibre.

---

### « Les aimants qui sont censés diriger le "corps creux rigide" sont des "aimants magiques" qui agissent sur le corps quand tu veux, et ne l’affectent plus quand tu ne veux pas. Si l’aimant est assez fort pour tirer le corps à travers une trappe à ressort et sur le côté jusqu’à ce qu’il flotte, il attirera toujours le corps et le maintiendra collé. »

J’imaginais, pour la trappe du bas par exemple, une force magnétique qui aide au passage de la trappe. La masse subit la gravité donc arrive avec un poids et une vitesse sur la trappe et doit l’ouvrir tout en repoussant l’eau au moment de l’ouverture de la trappe car l’eau agit comme une résistance sous cette trappe. Donc pour permettre cela j’ai ajouté un aimant pour gagner assez de force et pour que :

**F_air + (m × v) + F_aimant > F_eau + F_ressort + F_recul + F_chambre_tampon**

- F_air : Pression colonne d’air × surface de la trappe
- (m × v) : Impulsion de la masse (poids × vitesse au moment du contact)
- F_aimant : Force d’attraction magnétique agissant uniquement sur la masse
- F_eau : Résistance dynamique de l’eau (quasi instantanée)
- F_chambre_tampon : pression de la chambre tampon (qui augmente pendant l’ouverture trappe basse et diminue quand la trappe basse se referme ou quand le poids change de colonne trappe haute)
- F_ressort : Force du ressort maintenant la trappe fermée
- F_recul : Force à compenser si l’aimant est déplacé mécaniquement

Et pour que cela marche il faut que F_aimant < flottabilité après immersion dans l’eau.

Soit en ayant un aimant faible, soit en gérant la distance d’attraction (quand la trappe s’ouvre déplacer l’aimant mécaniquement pour contrôler sa force)

Et pour la trappe haute :

**F_eau + F_aimant + F_chambre_tampon > F_air + F_ressort + F_recul**

- L’air étant compressible, il génère une résistance modérée
- La pression de l’eau (incompressible) joue un rôle déterminant
- La poussée d’Archimède doit être suffisante pour compenser la résistance globale
- Et il faut que F_aimant < la force gravitationnelle subie par la masse

---

### « Comment tires-tu de l’énergie de ça ? »

Pour le moment je ne tire aucune énergie, j’essaye de voir si cela peut tourner quelques cycles, trouver les problèmes et les résoudre puis j’ajouterai un moyen de récupérer une énergie faible à un endroit non critique (exemple : si la trappe haute peut encaisser quelques newtons de résistance supplémentaires, j’ajoute un système à ce niveau).

---

### « Comment l’air et l’eau retournent dans leur colonne respective ? Car à chaque ouverture de trappe une partie de l’eau et de l’air change de colonne. »

Je vais essayer d’expliquer comment je voyais le transfert de l’eau et de l’air dans ce système.

Quand une trappe s’ouvre, de l’air va s’engouffrer dans la colonne d’eau, oui, et il va monter en haut de la colonne d’eau où un purgeur est installé et qui éjecte cet air à l’extérieur du système. Ce processus crée un vide en haut de la colonne d’eau une fois que l’air n’y est plus.

Au même moment que l’air va dans la colonne d’eau, l’eau elle va dans la colonne d’air. Ce qui fait que de l’eau s’accumule en bas de la colonne d’air.

Avec l’aide :
- de l’air qui rentre dans cette colonne pour équilibrer la pression interne (de l’air rentre car de l’air a été éjecté par le purgeur donc moins d’air dans le système),
- du poids tombant dans la colonne d’air de manière cyclique,
- et du vide créé dans la colonne d’eau,

…cela peut apporter l’énergie nécessaire pour repousser l’eau via une trappe unidirectionnelle (air impulse leak ejector) dans sa colonne initiale.

C’est comme cela que je voyais le déplacement de l’eau et de l’air dans ce système. 

---

Si quelque chose ne va pas ou est mal compris de ma part, je suis ouvert à toute critique pour avancer.