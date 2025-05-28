# Guide de Solution : "Le Mystère de PixelWave"

> ⚠️ **ATTENTION** : Ce guide est réservé aux organisateurs du challenge, aux participants qui ont terminé, ou à ceux qui ont décidé d'abandonner. Ne l'ouvrez pas si vous souhaitez relever le défi !

<details>
<summary>🔐 Guide de Solution (Cliquez pour révéler)</summary>

## Description du Challenge
Un développeur passionné de photographie a laissé des indices sur son identité à travers différents canaux en ligne. Votre mission est de retrouver son identité complète en utilisant les techniques d'OSINT.

## Structure du Challenge

### 1. Site PhotoFrame (pixelwavelyon.github.io/PhotoFrame)
- Site web statique hébergé sur GitHub Pages
- Design moderne avec CSS personnalisé
- Structure de fichiers :
  - `index.html` : Page d'accueil
  - `about.html` : Page À propos
  - `assets/` : Dossier contenant CSS et images
  - `assets/css/style.css` : Styles du site
  - `assets/images/` : Images du site

### 2. Challenge OSINT
- Forum statique simulant un post de développeur
- Fichiers inclus :
  - `index.html` : Page du forum
  - `styles.css` : Styles du forum
  - `images/photo_cafe.png` : Photo du café avec métadonnées
  - `robots.txt` : Contient des indices techniques
  - `sitemap.xml` : Contient des liens et métadonnées
  - `README.md` : Description du challenge

### 3. Réseaux sociaux
- Twitter : @PixelWaveLyon
  - Photo de profil cohérente
  - Tweets sur le développement
  - Localisation à Lyon
- Email : pixelwavelyon@protonmail.com

## Création technique du challenge

### 1. Image du café
- Source : Capture d'écran Google Maps du Café 203, place Saint-Paul, Lyon
- Métadonnées ajoutées avec ExifTool :
```bash
exiftool -GPSLatitude="45.7589024" -GPSLongitude="4.8269958" -GPSAltitude="0" \
         -DateTimeOriginal="2024:03:15 14:30:00" \
         -Author="PixelWaveLyon" \
         -Copyright="© 2024 PixelWaveLyon" \
         -Description="Photo prise au Cafe 203, place Saint-Paul, Lyon" \
         -Software="VS Code" \
         -UserComment="Developpement de PhotoFrame - Cafe 203, Lyon" \
         -charset iptc=UTF8 -charset exif=UTF8 images/photo_cafe.png
```
- Les coordonnées GPS correspondent exactement au Café 203
- La date et l'heure sont cohérentes avec le post du forum
- Les métadonnées incluent des indices sur l'identité du développeur

### 2. Site PhotoFrame
- Hébergé sur GitHub Pages
- Design moderne avec CSS personnalisé
- Structure de fichiers organisée
- Liens vers les réseaux sociaux
- Mentions du Café 203 dans le contenu

### 3. Réseaux sociaux
- Twitter créé avec le pseudo @PixelWaveLyon
- Photo de profil cohérente site/github/twitter
- Tweets sur le développement de PhotoFrame
- Localisation à Lyon
- Email ProtonMail créé : pixelwavelyon@protonmail.com

## Étapes de résolution

### Étape 1 : Analyse du post sur le forum
- Le post mentionne le "Café 203" à Lyon, place Saint-Paul
- L'image montre un café avec une date visible sur un journal (15/03/2024)
- Le développeur mentionne son projet "PhotoFrame" sur GitHub

### Étape 2 : Recherche du pseudo
- Recherche "PixelWave" sur GitHub
- Trouver le dépôt "PhotoFrame"
- Analyser le fichier README.md du projet qui contient une adresse email

### Étape 3 : Analyse des métadonnées
- L'image du café contient des coordonnées GPS (45.7589024, 4.8269958)
- Les métadonnées révèlent :
  - Date et heure : 15/03/2024 14:30:00
  - Auteur : PixelWaveLyon
  - Description : "Photo prise au Cafe 203, place Saint-Paul, Lyon"
  - Logiciel utilisé : VS Code
  - Commentaire : "Developpement de PhotoFrame - Cafe 203, Lyon"
- Le fichier sitemap.xml contient des liens vers les réseaux sociaux

### Étape 4 : Vérification sur les réseaux sociaux
- Le même pseudo est utilisé sur Twitter (@PixelWaveDev)
- Les posts récents confirment la localisation à Lyon
- La même photo de profil que sur le site

## Solution finale
- **Pseudo :** PixelWave
- **Localisation :** Lyon, France (Vieux Lyon)
- **Profession :** Développeur web / Photographe amateur
- **Projets :** PhotoFrame (application de gestion de photos)
- **Réseaux sociaux :** GitHub, Twitter (@PixelWaveDev)
- **Contact :** pixelwave@protonmail.com

## Techniques OSINT utilisées
1. Analyse des métadonnées d'image (EXIF)
2. Recherche de pseudos sur les réseaux sociaux
3. Analyse des fichiers techniques (robots.txt, sitemap.xml)
4. Géolocalisation via coordonnées GPS
5. Recherche croisée d'informations

## Notes techniques pour les organisateurs
Ce challenge utilise uniquement des services gratuits et existants :
- GitHub Pages pour l'hébergement
- ProtonMail pour l'email (gratuit)
- Twitter et GitHub pour les réseaux sociaux
- Google Maps pour l'image du café
- ExifTool pour la modification des métadonnées

## Niveaux de difficulté des indices

### Niveau 1 (Débutant)
- Pseudo "PixelWave" sur le forum
- Localisation à Lyon
- Projet PhotoFrame sur GitHub

### Niveau 2 (Intermédiaire)
- Métadonnées de l'image du café
- Coordonnées GPS dans le sitemap.xml
- Liens vers les réseaux sociaux

### Niveau 3 (Avancé)
- Email ProtonMail dans robots.txt
- Date et heure précises dans les métadonnées
- Croisement des informations entre les plateformes

## Points de vérification détaillés

### Configuration technique
- [ ] L'image photo_cafe.png contient toutes les métadonnées EXIF
- [ ] Le site GitHub Pages est accessible
- [ ] Les liens dans sitemap.xml sont valides
- [ ] Le robots.txt contient les bonnes informations
- [ ] Les styles CSS sont correctement appliqués

### Contenu et cohérence
- [ ] Les dates sont cohérentes entre les différentes sources
- [ ] Le pseudo est utilisé de manière cohérente
- [ ] Les localisations correspondent
- [ ] Les projets mentionnés sont accessibles
- [ ] Les profils sociaux sont liés entre eux & existants

## Variantes possibles

### Variante 1 : Challenge simplifié
- Supprimer certaines métadonnées de l'image
- Réduire le nombre de plateformes sociales
- Simplifier les fichiers techniques

### Variante 2 : Challenge avancé
- Ajouter des indices dans le code source
- Créer des faux profils supplémentaires
- Ajouter des métadonnées plus complexes

### Variante 3 : Challenge en équipe
- Diviser les indices entre différents fichiers
- Créer des rôles spécifiques (recherche web, analyse d'images, etc.)
- Ajouter des éléments de collaboration

## Adaptation au contexte
Le challenge peut être adapté selon :
- Le niveau des participants
- Le temps disponible
- Les objectifs pédagogiques
- Les contraintes techniques
- Le contexte d'utilisation (formation, compétition, etc.)

</details> 