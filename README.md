# 🧮 BitMatrix · MC88 — Convertisseur de Bases & IEEE 754

**BitMatrix** est un convertisseur radical de bases numériques (décimal, binaire, hexadécimal) avec un calculateur **IEEE 754** complet (simple et double précision) et des opérations arithmétiques en binaire/hexadécimal. L'interface cyber-luxueuse avec pluie de matrice animée fonctionne entièrement dans votre navigateur.

---

## 📋 Prérequis

1. Un navigateur web moderne (Chrome, Firefox, Edge, Safari, Brave, Opera)
2. Aucune connexion Internet requise après le chargement initial
3. Aucune installation de logiciel nécessaire

---

## 🚀 Guide d'installation

### Étape 1 : Télécharger le fichier
1. Téléchargez le fichier `bitmatrix.html` sur votre ordinateur
2. Placez-le dans un dossier de votre choix (ex : `C:\BitMatrix\`)

### Étape 2 : Lancer l'application
- **Méthode simple** : Double-cliquez sur le fichier
- **Méthode alternative** : Faites un clic droit → « Ouvrir avec » → choisissez votre navigateur

---

## 🎯 Fonctionnalités principales

### 🔷 1. Convertisseur Universel

Convertit instantanément entre trois bases numériques :
- **Décimal** (base 10) : ex. `10.625`
- **Binaire** (base 2) : ex. `1010.101`
- **Hexadécimal** (base 16) : ex. `A.A`

**Conversion automatique :**
- Saisissez dans n'importe quel champ → les deux autres se mettent à jour
- Les **étapes de conversion** sont affichées en temps réel
- Supporte les nombres fractionnaires (partie décimale)

**Méthode de conversion binaire :**
1. Partie entière : divisions successives par 2
2. Partie fractionnaire : multiplications successives par 2
3. Limite : 20 bits pour la partie fractionnaire

---

### 🧮 2. Calculateur IEEE 754

Convertit un nombre réel en sa représentation binaire flottante :

**Simple précision (32 bits) :**
| Composant | Bits | Description |
|-----------|------|-------------|
| **Signe (S)** | 1 bit | 0 = positif, 1 = négatif |
| **Exposant (E)** | 8 bits | Biais de 127 |
| **Mantisse (M)** | 23 bits | Partie fractionnaire normalisée |

**Double précision (64 bits) :**
| Composant | Bits | Description |
|-----------|------|-------------|
| **Signe (S)** | 1 bit | 0 = positif, 1 = négatif |
| **Exposant (E)** | 11 bits | Biais de 1023 |
| **Mantisse (M)** | 52 bits | Partie fractionnaire normalisée |

**Affichage :**
- Valeur hexadécimale 32 bits : `0x40B80000`
- Valeur hexadécimale 64 bits : `0x4017000000000000`
- Décomposition visuelle : S | E | M avec couleurs distinctes

**Exemple :**
- Entrée : `5.75`
- 32 bits : `0x40B80000`
- Décomposition : `S:0 E:10000001 M:01110000000000000000000`

---

### ⚙️ 3. Opérations Arithmétiques

Effectue des calculs directement en binaire ou hexadécimal :

**Opérations supportées :**
- **Addition** (+)
- **Soustraction** (−)
- **Multiplication** (×)
- **Division** (÷)

**Fonctionnement :**
1. Saisissez deux opérandes (binaire ou hexadécimal)
2. Choisissez l'opérateur
3. Cliquez sur `=`
4. Le résultat s'affiche dans la même base

**Exemple :**
- `1010.1 + 10.1 = 1101.0` (binaire)
- `A.F + 1.1 = C.0` (hexadécimal)

**Gestion des erreurs :**
- Division par zéro → message d'erreur
- Format invalide → message d'avertissement

---

### 📋 4. Historique des conversions

- Les **12 dernières conversions** sont sauvegardées
- Stockage local persistant (survit au rechargement)
- **Cliquez** sur un élément pour le recharger
- Bouton **Clear** pour effacer l'historique

---

## 📖 Guide d'utilisation détaillé

### 🔹 Étape 1 : Convertir un nombre

1. Repérez la section **« Universal Converter »**
2. Saisissez votre nombre dans l'un des trois champs :
   - **Decimal** : `10.625`
   - **Binary** : `1010.101`
   - **Hexadecimal** : `A.A`
3. Les deux autres champs se remplissent automatiquement
4. Les **étapes de conversion** s'affichent en dessous

### 🔹 Étape 2 : Calculer IEEE 754

1. Repérez la section **« IEEE 754 Floating-Point »**
2. Saisissez un nombre réel (ex. `5.75` ou `-12.625`)
3. Les résultats s'affichent instantanément :
   - Valeur hexadécimale 32 bits
   - Décomposition Signe/Exposant/Mantisse
   - Valeur hexadécimale 64 bits

### 🔹 Étape 3 : Effectuer une opération

1. Repérez la section **« Arithmetic (Bin / Hex) »**
2. Saisissez le premier opérande
3. Choisissez l'opérateur (+, −, ×, ÷)
4. Saisissez le second opérande
5. Cliquez sur `=`
6. Le résultat et les étapes s'affichent

### 🔹 Étape 4 : Utiliser l'historique

- Les conversions récentes apparaissent dans la barre latérale
- Cliquez sur un élément pour le recharger dans le convertisseur
- Utilisez **Clear** pour vider l'historique

---

## 🛠️ Guide de dépannage

### Problème 1 : « Invalid decimal number »

**Cause** : Le nombre décimal contient des caractères non numériques.

**Solution** :
- Utilisez uniquement des chiffres (0-9) et un point décimal
- Exemple valide : `10.625`
- Exemple invalide : `10,625` (virgule au lieu du point)

---

### Problème 2 : « Invalid binary »

**Cause** : Le nombre binaire contient des chiffres autres que 0 et 1.

**Solution** :
- Utilisez uniquement `0` et `1`
- Exemple valide : `1010.101`
- Exemple invalide : `1020.101`

---

### Problème 3 : « Invalid hex »

**Cause** : Le nombre hexadécimal contient des caractères hors de 0-9 et A-F.

**Solution** :
- Utilisez uniquement `0-9` et `A-F` (ou `a-f`)
- Exemple valide : `A.F`
- Exemple invalide : `G.5`

---

### Problème 4 : Division par zéro

**Cause** : Le second opérande est égal à zéro.

**Solution** :
- Vérifiez que le diviseur n'est pas zéro
- En binaire : `0` ou `0.0`
- En hexadécimal : `0` ou `0.0`

---

### Problème 5 : Le résultat IEEE 754 est « Invalid »

**Cause** : Le nombre saisi n'est pas un nombre réel valide.

**Solution** :
- Utilisez un nombre décimal valide (ex. `5.75`)
- Évitez les caractères spéciaux
- Accepte les nombres négatifs (ex. `-12.625`)

---

### Problème 6 : L'historique ne se sauvegarde pas

**Cause** : Le stockage local est désactivé ou en navigation privée.

**Solution** :
- Vérifiez que le stockage local est activé
- En navigation privée, l'historique sera réinitialisé
- C'est un comportement normal

---

### Problème 7 : La pluie de matrice ralentit l'appareil

**Cause** : L'animation canvas consomme des ressources sur les appareils anciens.

**Solution** :
- L'opacité est réduite automatiquement sur mobile (0.25)
- Sur mobile, la taille de police est réduite
- Fermez les autres onglets gourmands

---

## 📊 Exemples de conversion

### Exemple 1 : Décimal → Binaire → Hexadécimal

**Entrée :** `10.625` (décimal)

**Résultat :**
- Binaire : `1010.101`
- Hexadécimal : `A.A`

**Étapes :**
- Partie entière : `10₁₀ = 1010₂`
- Partie fractionnaire : `0.625₁₀ = 0.101₂`
- Hexadécimal : `10₁₀ = A₁₆`, `0.625₁₀ = 0.A₁₆`

---

### Exemple 2 : IEEE 754 Simple Précision

**Entrée :** `5.75`

**Résultat :**
- Hex 32 bits : `0x40B80000`
- Signe : `0` (positif)
- Exposant : `10000001` (129 - 127 = 2)
- Mantisse : `01110000000000000000000`

**Vérification :**
`(-1)⁰ × 1.0111₂ × 2² = 1.4375 × 4 = 5.75`

---

### Exemple 3 : Arithmétique Binaire

**Entrée :** `1010.1 + 10.1`

**Résultat :**
- Décimal : `10.5 + 2.5 = 13.0`
- Binaire : `1101.0`

---

## 📄 Copyright

**© 2026**  
📧 mohamed005cheikh@gmail.com  
**Créé par MC**  
**Tous droits réservés**

---

## 🔗 Formules techniques

### Conversion Décimal → Binaire (fractionnaire)
---

## ✅ Fonctionnalités techniques

- **Conversion bidirectionnelle** entre 3 bases
- **Étapes de conversion** détaillées en temps réel
- **IEEE 754** simple et double précision
- **Arithmétique** en binaire et hexadécimal
- **Historique persistant** (12 entrées)
- **Pluie de matrice** animée en arrière-plan
- **Design responsive** mobile-first
- **Glassmorphism** avec effets de flou
- **Effets de lueur** néon améthyste
- **Défilement personnalisé** avec lueur violette

---

**Bonnes conversions ! 🧮✨**
