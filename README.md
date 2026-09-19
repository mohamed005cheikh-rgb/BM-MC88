<div align="center">

🧮 BitMatrix — MC88

Voir les nombres sous toutes leurs formes.

<br />

✨ Nouvelle version — entièrement repensée.
Plus fluide, plus claire, plus agréable à utiliser. Le même outil, en mieux.

</div>

---

👋 Bienvenue

BitMatrix est un petit atelier pour ceux qui aiment comprendre ce qui se passe vraiment sous le capot d'un nombre.

Vous entrez une valeur — dans n'importe quelle base — et vous la voyez apparaître sous toutes ses autres formes : binaire, hexadécimal, décimal. Vous voulez savoir comment un ordinateur stocke 5.75 en mémoire ? Le calculateur IEEE 754 vous le montre, bit par bit. Vous voulez additionner deux nombres en binaire, à la main ? L'outil le fait pour vous, et vous montre chaque étape.

Tout fonctionne dans votre navigateur. Pas d'installation, pas de serveur, pas de compte. Vous ouvrez, vous explorez, vous fermez.

---

🎉 Ce qui a changé

Cette version n'est pas une simple retouche — c'est une refonte complète de l'expérience. Voici ce que vous allez remarquer dès la première seconde :

Une interface enfin à la hauteur.
Fini les petits symboles génériques et les icônes qui jurent. Chaque bouton, chaque section, chaque indicateur a désormais sa propre identité visuelle, dessinée sur mesure. L'ensemble respire, s'aligne, et se laisse parcourir du regard sans effort.

Trois espaces, une seule logique.
Le convertisseur, le calculateur IEEE 754 et les opérations arithmétiques vivent maintenant chacun dans leur propre onglet. Vous passez de l'un à l'autre d'un clic, sans faire défiler ni chercher. Chaque outil a son espace, chaque espace a sa fonction.

Une navigation qui glisse.
Les animations sont partout, mais discrètes — un onglet qui se déplace, un résultat qui pulse doucement quand il change, un champ qui s'illumine quand vous le touchez. Rien de tapageur. Juste ce qu'il faut pour que l'outil se sente vivant.

Zéro lag, même sur mobile.
La pluie de matrice en arrière-plan a été allégée pour ne plus jamais ralentir l'appareil. Les animations s'adaptent à la puissance de votre machine, et si vous préférez le calme, tout se met en pause quand vous ne regardez pas.

Un historique qui prend de la place.
Vos trente dernières conversions restent à portée de main dans la barre latérale (au lieu de douze). Un clic, et n'importe quelle entrée revient dans le convertisseur. Un bouton, et tout s'efface.

Des détails qui comptent.
Chaque résultat peut être copié d'un seul geste. Chaque bit de la représentation IEEE 754 est coloré selon sa fonction (signe, exposant, mantisse). Chaque erreur vous dit précisément ce qui ne va pas, sans jargon inutile.

---

✨ Ce que vous trouverez

Convertir, dans les trois sens.
Vous tapez 10.625 en décimal, et vous voyez aussitôt 1010.101 en binaire et A.A en hexadécimal. Vous tapez dans n'importe quel champ — les deux autres se mettent à jour tout seuls. Les nombres à virgule sont acceptés, et les étapes du calcul s'affichent pour que vous compreniez d'où vient chaque chiffre.

Voir un nombre flottant, bit par bit.
Entrez 5.75, et l'outil vous montre comment il est réellement stocké en mémoire — en simple précision (32 bits) comme en double précision (64 bits). Le signe, l'exposant, la mantisse : chacun affiché séparément, avec sa valeur hexadécimale complète (0x40B80000 pour 5.75 en 32 bits). Chaque partie est colorée pour que votre œil distingue immédiatement les trois zones. Une façon limpide de comprendre la norme IEEE 754 sans se perdre dans un manuel.

Calculer directement en binaire et en hexadécimal.
Addition, soustraction, multiplication, division — sur des nombres écrits en base 2 ou en base 16. Vous entrez les deux opérandes, vous choisissez l'opérateur, et le résultat s'affiche dans la même base, avec les étapes détaillées. Vous basculez entre binaire et hexadécimal d'un clic, sans retaper vos valeurs.

Un historique qui se souvient.
Vos trente dernières conversions restent dans la barre latérale, prêtes à être rechargées d'un clic. Vous pouvez les comparer, y revenir plus tard, ou tout effacer d'un seul bouton.

Une ambiance qui invite à jouer.
Une pluie de matrice animée en arrière-plan, une palette améthyste, des lueurs discrètes — l'outil est aussi agréable à regarder qu'à utiliser. Et sur mobile, tout s'allège automatiquement pour rester fluide.

---

🧭 Comment ça marche

1. Convertir un nombre.
Cherchez l'onglet Converter. Tapez votre valeur dans le champ qui vous arrange — décimal, binaire ou hexadécimal. Les autres se remplissent immédiatement, et les étapes apparaissent juste en dessous. Un bouton Reset efface tout si vous voulez repartir de zéro.

2. Explorer un flottant.
Passez à l'onglet IEEE 754, puis entrez un nombre réel (positif ou négatif). Vous obtenez aussitôt sa représentation 32 bits et 64 bits, avec la décomposition Signe / Exposant / Mantisse colorée pour bien distinguer chaque partie, et chaque hexadécimal prêt à être copié.

3. Faire une opération.
Ouvrez l'onglet Arithmetic, choisissez votre base (binaire ou hexadécimal), entrez le premier opérande, sélectionnez l'opérateur, entrez le second, et cliquez sur Compute. Le résultat s'affiche dans la même base que vos entrées, accompagné des étapes de calcul.

4. Retrouver une conversion.
Cliquez sur n'importe quelle entrée de l'historique pour la recharger dans le convertisseur. Le bouton de la corbeille vide la liste quand vous voulez repartir à zéro.

C'est tout. L'outil ne demande rien, ne garde rien ailleurs, et ne vous impose aucune étape inutile.

---

🛠️ Petits coups de main

« Invalid decimal number » ?
Vérifiez que vous n'avez utilisé que des chiffres et un point décimal. La virgule n'est pas acceptée — c'est 10.625, pas 10,625.

« Invalid binary » ?
En binaire, il n'existe que deux chiffres : 0 et 1. Si vous voyez un 2, c'est qu'il y a un problème.

« Invalid hex » ?
En hexadécimal, on va de 0 à 9, puis de A à F. Les lettres G et au-delà n'existent pas dans cette base.

Le résultat IEEE 754 affiche Invalid ?
Vérifiez que votre entrée est bien un nombre réel — par exemple 5.75 ou -12.625. Les caractères spéciaux ne sont pas acceptés.

L'historique disparaît ?
En navigation privée, le stockage local est désactivé — c'est normal. En fenêtre normale, vos conversions restent tant que vous ne videz pas le cache.

La pluie de matrice ralentit l'appareil ?
Sur mobile, l'animation s'allège automatiquement. Si cela reste gênant, fermez les autres onglets gourmands — ou laissez l'onglet ouvert sans y toucher, il se calme tout seul.

Les animations me dérangent ?
Si votre système est réglé pour réduire les animations, BitMatrix les désactive automatiquement. Le confort avant tout.

---

<div align="center">

📞 Une question, une idée ?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_72_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white

<br />

Bonnes conversions.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

</div>
